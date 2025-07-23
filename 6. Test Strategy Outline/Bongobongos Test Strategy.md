Test Strategy
Purpose
This test strategy document intends to outline all the activities that will take place during testing of the 'Place Bet' feature. The document will discuss the test approach, the execution strategy and test management.

Objective
Verifying the ability to place a straight bet, check bet slip and receives confirmations effortlessly. This testing covers the straight bet betting, ensuring smooth operations under all scenarios, including peak usage.

Scope
IN-SCOPE: 
    •	Ability to place a single straight bet.
    •	Ability to view bet slip
    •	Bet Success confirmation
OUT-OF-SCOPE:
    •	Testing Login and Registration
    •	Testing other betting options including parlays and live betting,
    •	Testing deposit and withdrawal processes
    •	Testing inclusion of Promotions
    •	Testing KYC Pass

Test Strategy
TEST ASSUMPTIONS:
    •	User Age qualifies them to bet
    •	User is verified
    •	User has funds
    •	User is KYC Passed
DATA APPROACH:
    •	Testers will use the boundary value analysis vs equivalence partitioning techniques to generate data
 
LEVEL OF TESTING:
--------------------------------------------------------------------------------------------------------
| Test Type                                     |   Description                 |   Responsible Parties |
--------------------------------------------------------------------------------------------------------
|   Unit Testing                                |•	White box                   |                       |
|                                               |•	Functions as expected       |                       |
|                                               |•	Performance Testing	        |                       |
|   Functional and Non Functional Testing       |•	Black Box                   |                       |
|                                               |•	Usability testing           |                       |
|                                               |•	Accessibility testing       |                       |	
|    System Testing	                            |•	End to end testing	        |                       |
|    Acceptance Testing	                        |•	Cover real-world scenarios	|                       |
---------------------------------------------------------------------------------------------------------

UNIT TESTING:
White Box
    •	Validate API responses
        •	Bet is saved successfully
        •	Ability to get bet slip details
        •	Events are loaded
Performance Testing
        •	Performance Testing:  Simulate loading of the betting events page
        •	Load Testing: Simulate peak number of users placing betting.
FUNCTIONAL TESTING:
Black Box
    •	Ability to place a single straight bet.
        •	Find Event: Validate user is able to find an active event to bet on
        •	Wager amount : Validate user is able enter their wager amount
        •	Submit bet: Validate user is able to submit their bet
    •	Bet Success confirmation
        •	Bet confirmation: Validate a confirmation popup appears on the screen
    •	Ability to view bet slip
        •	Bet Slip: Validate user is able to view their betting slip
Usability Testing
    •	Validate the betting app is available and user is able to complete a straight bet.
        o	Find an event
        o	Enter wager
        o	Submit bet
Accessibility testing
    •	Validate user is able to interact with the application elements
 
USER ACCEPTANCE TESTING:
Beta Testing
    •	Allow user to run scenarios on the application

REGRESSION TESTING:
Manual
    •	Confirm no key features have been affected by the new change
Automation
    •	Run existing regression
    •	Add new feature to regression

Environment Requirements
TEST ENVIROMENTS:
    •	Development environment 
        o	Development
        o	Feature review
    •	 Staging Environment
        o	Test Execution
        o	Beta testing
TOOLS:
    •	Emulators
    •	JMeter

Execution Strategy
ENTRY CRITERIA:
---------------------------------------------------------------------------------------------------------------------
|   Entry Criteria                                                      |    Tester     |   Test Lead   |   Notes   |
---------------------------------------------------------------------------------------------------------------------
|   Code has been merged successfully                                   |               |               |           |
|   Development has completed unit testing                              |               |               |           |
|   Feature Review has been done                                        |               |               |           |   
|   Tester Merged Changes to Staging environment Successfully           |               |               |           |			
|   Test Environment(s) is available                                    |               |               |           |			
|   Test Data is available                                              |               |               |           |			
|   Test Cases are completed, reviewed and approved by the testing team |               |               |           |
---------------------------------------------------------------------------------------------------------------------     			

 
EXIT CRITERIA:
----------------------------------------------------------------------------------------------------------------------------
| Exit Criteria                                                                     |   Tester  |   Test Lead   |   Notes   |
-----------------------------------------------------------------------------------------------------------------------------
| 100% Test Scripts executed                                                        |           |               |           |
| 90% pass rate of regression test scripts                                          |           |               |           |
| No open Critical and High Severity Defects                                        |           |               |           |
| All remaining defects are either cancelled or documented                          |           |               |           |
  as requests for a future release.	                                                            		        
| All expected and actual results are captured and documented with the test script  |           |               |           |
| All test metrics collected based on reports from daily and weekly status reports  |           |               |           |
| All defects logged in Defect Tracker/Spreadsheet                                  |           |               |           |
| Test environment cleanup completed and a new back up of the environment           |           |               |           |
----------------------------------------------------------------------------------------------------------------------------

Risks & Mitigations 
RISKS:
    •	Payment processing systems
        •	Failed transactions
        •	Double charges
Mitigations:
    •	Implement background retries until a certificatory code is found before displaying confirmation popup.















