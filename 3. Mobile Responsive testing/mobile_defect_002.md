
                                Global SQA Defect Report
--------------------------------------------------------------------------------------------------
Bug#: GSD15586

Title: GlobalSQA app image drag and drop functionality doesn’t work on mobile devices.

Description: Image Drag and Drop functionality is not working on all mobile
device platforms. Tested with IPhone X and Pixel 7 and in both devices dragging
the image to trash is not responding as expected. Issue is also visible on both app
versions (v1 and v2) and on the builds (#: IV5545255645 and IV1455445651).

Reporter: Sakhumzi Ncantswa

Date: 21-07-2025

Device: Device: Chrome DevTools emulator -  IPhoneX and Pixel 7

App Version: v1 and v2

Build#: IV5545255645 and IV1455445651

Steps to reproduce:
            1. Go to ‘https://www.globalsqa.com/’
            2. Navigate to Drag and Drop page via menu
                a. Click menu
                b. Click open ‘Tester’s Hub’ submenu
                c. Click open ‘Demo Testing Site’ submenu
                d. Click open Drag and Drop page
            3. Scroll down to photo manager tab
            4. Issue : Drag image to trash doesn’t work

Expected: User should be able to drag an image and drop in trash bin.

Priority: High

Severity: High – Issue is experienced in all mobile device platforms

Evidence:
Find screen video Gif in the evidence folder
path:   3. Mobile Responsive testing\defect_002_evidence - DraAndDropBug.gif