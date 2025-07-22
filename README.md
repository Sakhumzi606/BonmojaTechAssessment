# BonmojaTechAssessment
Bonmoja-Bongobongos Tech Assessment

#################
#     Postman   #
#################


Download github repositories
------------------------------------------------------------
    - Go to https://github.com/Sakhumzi606/BonmojaTechAssessment
    - download repository zip Or Clone
    - Repo Contains 6 folders
        1. Postman API
        2. Mobile Responsive testing
        3. Test Script Creation
        4.
        5. Defect Documentation
        6. Test Strategy Outline
How to get Postman
------------------------------------------------------------
    - Download postman  https://www.postman.com/downloads/
    - Install and setup a free account

How to run post man tests
------------------------------------------------------------
    - Open Postman
    - Click import Button 'Dro anywhere to import' window should open
    - Click Files or Folders to navigate to where you saved the Cloned 'BonmojaTechAssessment'folder
      OR Drag and Drop the 2 JSON Files
    - Postman request files should be loaded in your post man workspace
    - To run all the requests   - Select Folder
                                - Right click and click Run
                                - All your request should be ready to run
                                - Click Run BongobongosAPI
                                - Run Results will be displayed
    - Run single test - Expand the folder 'BongobongosAPI'
                                - Select request run
                                - Click Button Send
                                - Run Request Response wll be displayed
                                - Run Test Results will be displayed
Tests setup
-------------------------------------------------------------
    - Bongobongo's API is documented in the https://reqres.in/ website
    Request Endpoint
        - Base URL is https://reqres.in/
        - Each test url wil contain the base Url + the test Endpoint e.g '/api/login' 
    Authentication
      Token
        - For Authentication the tests are using a Bearer Token - stored in the enviroments variable
          referenced in the Request Authentication tab e.g '$(token)'
      API Ke
        - Strored as Key and Value in the Header tab
    Request Body
        - Stored under the Body > raw tab 
    Response Validation 
        - Is done using the javascrip under the Scripts tab

Run Responsive testing in CromeDevTools
---------------------------------------------------------------
    How to get Chrome
        - Should be install already in your PC
         OR
        - Download and install from https://www.google.com/chrome/
    Open Chrome
        - open DevTools 
            - Inside Page Right click > Click inspect
             Or
            - Press Keyboard F12 
    Change device mode
            - In the devTool header find icon 'Toggle Device Toolbar' 
              Click Icon to change from Web to mobile 
              OR 
              use keyboar comand CTRL + Shift and M

Setup android emulator
-----------------------------------------------------------------
    -Simpler way to install is to download with android studio 
       PreRequirement
          - latest java - JAVA_HOME
          - Latest SE runtime - JRE_HOME
          - Latest JDK - Add To Path
        Map them to your machine enviromental variables  
    - Follow instructions
       https://medium.com/@queen_shecoder/getting-started-with-setting-up-an-emulator-in-android-studio-8b573dd2326f

    Start emulator
        - Open Android Studio
        - Device Manager Click +icon and Select Create Virtual Device
        - Select device type and download
        - After installing device should be ready
        - click Start icon 
    Install APK
        Drag and drop on the device


Any prerequisites
    - Latest
        Chrome browser, 
        Android Studio,
        Postman version
