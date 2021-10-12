# JumpCloud_QAAssignment_2021
Please read the JumpCloud_TestPlan.xls and the JumpCloudTest_PreRequsites.txt before interpreting the testing of the feature.

Documentation Folder:

Requirements are JumpCloud_ QA Assignment 2021.pdf
Test results plus reports are in the folder titled Testing.zip



# apiJumpCloud

apiJumpCloud is a robotframework based solution for testing JumpCloud_ QA Assignment 2021.pdf as well as it corespnds to the Automated (Column C) test cases in the Test Plan titled JumpCloud_TestPlan.xls.  

## Installation

**Please ensure you downloaded and ran the password hashing application. Please see JumpCloud_ QA Assignment 2021.pdf for instructions**

To run the automation suite install the following:

Python 3.6 or higher
Pycharm IDE

▪ Install Following Libraries using Terminal

➢ robot framework
➢ requests
➢ robotframework-requests
➢ robotframework-jsonlibrary

Open the Project titled apiJumpCloud

Go to Pycharm > Preferences > Project: apiJumpCloud > Project Interpreter
Hit the plus symbol at tht bottom right and add the previosu libraries into your project

Go to terminal and go to the directory titled TestCases

Follow the test plan title JumpCloud_TestPlan.xls and run the commands correposning to the given test case

## Execution

Open Terminal
robot <FileNmae>

## Log examples

(venv) Kirondes-MacBook-Pro-2:TestCases kirondechery$ robot Jump_TC_POST_Request.robot
==============================================================================
Jump TC POST Request                                                          
==============================================================================
Get stats number prior to post request Post 4                         .....{"TotalRequests":0,"AverageTime":0}
Get stats number prior to post request Post 4                         | PASS |
------------------------------------------------------------------------------
Pos:Post Request for password angrymonkey Post 5                      ...{'password': 'angrymonkey'}
[ WARN ] Keyword 'RequestsLibrary.Post Request' is deprecated. Please use `POST On Session` instead.
Pos:Post Request for password angrymonkey Post 5                      ..{'Date': 'Tue, 12 Oct 2021 16:53:42 GMT', 'Content-Length': '1', 'Content-Type': 'text/plain; charset=utf-8'}
..5.009
Pos:Post Request for password angrymonkey Post 5                      | PASS |
------------------------------------------------------------------------------
Pos:Post Request for password "abcd1234" Post 6                       ...{'password': 'abcd1234'}
[ WARN ] Keyword 'RequestsLibrary.Post Request' is deprecated. Please use `POST On Session` instead.
Pos:Post Request for password "abcd1234" Post 6                       ..{'Date': 'Tue, 12 Oct 2021 16:53:48 GMT', 'Content-Length': '1', 'Content-Type': 'text/plain; charset=utf-8'}
Pos:Post Request for password "abcd1234" Post 6                       | PASS |
------------------------------------------------------------------------------
Neg: Post Request with incorrect headers Post 6a                      ...{'password': 'abcd1234'}
[ WARN ] Keyword 'RequestsLibrary.Post Request' is deprecated. Please use `POST On Session` instead.
Neg: Post Request with incorrect headers Post 6a                      ..{'Content-Type': 'text/plain; charset=utf-8', 'X-Content-Type-Options': 'nosniff', 'Date': 'Tue, 12 Oct 2021 16:53:53 GMT', 'Content-Length': '16'}
Neg: Post Request with incorrect headers Post 6a                      | PASS |
------------------------------------------------------------------------------


#Report path from root (Folder Titled Reports are in the zip called testing)

TestCases/report.html
Right click and choose open in browser
