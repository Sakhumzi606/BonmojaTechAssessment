1.	Login → Update User Profile → Logout (happy path) 
   
Preconditions: 
•	User exists
•	Authentication pass

Scenario: Update user profile information
    Given I have a valid user token
    When I update the my user profile with the following information
      | name       | job         	|
      | John Doe | Software Dev 	|
    Then I should receive a response with status code 200
    And the updated user profile should match the following
      | name       | job         	|
      | John Doe | Software Dev 	|
    Then the user logs out  

2.	Login with expired/invalid token (session handling) 

Preconditions: 
•	User exists
•	Authentication fail - invalid token

    Scenario: User access their profile with valid token
      Given I have an expired or invalid token
      When I attempt to access the user profile
      Then I should receive a response with status code 401
      And the response should indicate that the token is invalid or expired

3.	Update Profile with missing required fields 

Preconditions: 
•	User exists
•	Authentication fail - invalid APIKEY

  Scenario: User attempts to update profile with invalid data
    Given I have an invalid user APIKEY
    When I attempt to update my user profile with the following information
      | name     	| job             	 |
      | John Doe 	|   Software Dev|
    Then I should receive a response with status code 400
    And the response should contain the following error message
      | error | "Invalid API key." |
4.	Fetch User List with invalid pagination parameters 

Preconditions: 
•	User exists
•	Authentication pass

  Scenario: Fetch User List with invalid pagination parameters
    Given I have a valid user APIKEY
    When I attempt to fetch the user list with invalid pagination parameters
      | page | 0 |
    Then I should receive a response with status code 404
    And the response should contain the following error message
      | error | "Invalid page number." |
