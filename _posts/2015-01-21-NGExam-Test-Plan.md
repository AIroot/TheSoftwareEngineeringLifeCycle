---
layout: post
title: Software Test Plan Outline
---
NGE Mobile Application Test Plan
Anuruddha I Jayasekara Pathiranage
Regis University
01/28/2017
Table of Contents
1.0
TEST PLAN IDENTIFIER………………………………………………………...
3
2.0
INTRODUCTION………………………………………………………………….
3


2.1
NATURE OF THE PROJECT………………………………………………
3


2.2
SYSTEM TEST OBJECTIVES AND SCOPE……………………………..
4




2.2.1
Test Objectives………………………………………………………
4




2.2.2
Testing Scope………………………………………………………..
4


2.3
RELATED DOCUMENTS………………………………………………….
5
3.0
ITEMS TO BE TESTED…………………………………………………………...
5
4.0
FEATURES…………………………………………………………………………
5


4.1
FEATURES TO BE TESTED……………………………………………….
5


4.2
FEATURES NOT TO BE TESTED…………………………………………
5
5.0
APPROACH………………………………………………………………………..
6


5.1
SOURCES OF SAMPLE……………………………………………………
6


5.2
TESTING TEAM……………………………………………………………
6


5.3
RECORD DOCUMENTING FOR TEST………………………………….
6


5.4
TEST STATUS………………………………………………………………
6


5.5
TEST TOOLS……………………………………………………………….
7


5.6
STOP TEST CRITERIA…………………………………………………….
7


5.7
TEST CASES……………………………………………………………….
7




5.7.1
USER GUIDE LINE………………………………………………..
7




5.7.2
CREATE NEW EVENT……………………………………………..
8




5.7.3
SET THE EXAM/COURSE START AND DUE DATE……………
11




5.7.4
SET THE ASSIGNMENT START AND DUE DATE……………..
13




5.7.5
SET THE REMAINDER OF 1% -100% COMPLETION………….
16




5.7.6
UPDATE EVENT……………………………………………………
18




5.7.7
DELETE EVENT……………………………………………………
22
6.0
PASS/FAIL CRITERIA……………………………………………………….........
23
7.0
SUSPENSION AND RESUMPTION CRITERIA………………………….……...
24
8.0
TEST DELIVERABLES……………………………………………………….......
24
9.0
TESTING TASKS………..………………………………………………………...
25
10.0
TESTING ENVIRONMENT……………………………………………………...
26
11.0
RESPONSIBILITIES……………………………………………………………...
26
12.0
STAFF AND TRAINING NEEDS………………………………………………...
27
13.0
SCHEDULING…………..………………………………………………………...
27
14.0
RISKS AND CONTINGENCIES………………………………………………...
27
15.0
APPROVAL………………………………………………………………………...
27


REFERENCE………………………………………………………........................
28


Test Plan Recognizer
QANGE001
Introduction
This section introduces the mobile application under test, providing basic background information, an overview, test objectives and scope. There is a list of related documents attached.
Nature of the Project
NGE is a mobile based Android mobile application to organize exam and courses in universities and any educational institutes for students and exam takers. This can  be used as an online or offline application based on user’s android device. NGE provides easy and well organized pre-design content for exam and courses. Users can create events for their exam and they can assign their target achievement as a grade or percentage of point. Then application provides guide lines to achieve their target in unique way according to the user. 
There is a notification system and progressing bar to indicate future action and past work for user. When user creates exam or course event, system will create local database and table for new event. After creating the event, user can notify what are the important things that have to focus those areas in exam or course. This notification works with time frame. The application provides multi task facility and if there are any past activities, those activities will use as past experiences to predict new event’ achievement. This function is more helpful to get a big motivation for success in event. 

Application Test Objectives and Scope
This test plan describes the application requirement, environment, activities, tasks, tools, costs, and schedules for system testing the NGE application.
Test Objectives
The objectives for application system testing are to validate the following sections:
Create and organize exam and course event
Notification based user activity
The test objectives are:
Ensure full functional areas act in accordance with each exam and courses with related institute.
The application is user friendly and easy to use.
The application meets its performance requirements.
The application can handle crash reporting and exception.   
User experience and user interface with different devices.

Test Scope
The project will test the version 1.0 release of the new application and will perform set of application tests including:
Functional Testing- Creation new course event, verification of real time progressing bar, viewing available event, notification system, input data validation, verification of past data identification with current event

Performance Testing – Event saving time, event delete time
Reliability Testing – Accuracy of data entry, completed records
Related Documents
User privacy agreement
Input data specification
Items To Be Tested
Application user’s guide line modules
Event creation modules
Real time notification modules
Completed event handling modules
Features
Features To Be Tested
Create and organize exam and course event
User guide line
Create new event
Update event
Delete event
Notification based user activity
Set the Assignment due date 
Set the course due date
Set the reminder for 50%, 75%, 95% competence 

Features Not To Be Tested
The Android operating system’s SQLITE database is not tested under this plan. This application run on Android API 15-24. This API compatibility in not tested in this plan. 

Approach
The NGE Android mobile development team does not have a separate testing group. Testing also should be done by mobile developer in the team. They have the necessary resources and a test environment to support their test effort. In the mobile application all items will be tested until requirements are satisfied and to ensure the software will work properly. There is well organized document handle system which save all test cause, specification for future testing.
Sources of Sample
The team will create dummy event as a user using virtual courses and exam due dates.
Testing team
The one main developer for NGE will be responsible for test case design, test execution, and the recording of test results. Other developer will provide assistance as needed. 
Record documenting for test
All test results will be recorded in a test log file and saved on the test file directory. All test failures will be captured in a problem report and given a severity grade level. 
Test Status
There is no automated test. The status of the test event will be reported and discussed with team. 
Test Tools
The following tools will be used to do test easier. Any tester has good training to use the tools. The tools are the following:
Android Emulator
Git version control system
Stop-Test Criteria
Stop testing is depend on defect level. The decision to stop the testing will be based on how many defects are discovered versus how many requirements are covered.
 Test Cases
User guide line
Feature Under Test: User Guide Line
Use Case: A new user can get idea about how to use the application to organizing their courses and exam. 
Working flow chart
Install the NGE app into the device. 
Click the app icon in the device
When the app open first UI display User guide lines step by step.
Expected Outcome Success:
Display the user guide line.
Guide line can be scrollable and clear to understand 
Guide line provides complete details about how to use the application
Expected Outcome Failure: 
Guide line is not displayed
Application view Error
Test Approach
Course catalog view is the main user interface that will show the course as list view. If there is an empty view (without any courses) it will display user guidelines.  There is an action bar that has delete icon to delete courses and past experiences icon to collect finished exams or courses. Finished courses can highlight to collect into the past experiences. Also Fab button will link to the edit view.
There is no valid input domain. The guide line creates and displays as a system default option. If the guide line is not displayed there is system error. 

Create new event
Feature Under Test: Create new event
Use Case: The user can add or edit courses into the app database using Course catalog view by pressing fab button or on courses icon.  Then it will open edit view to get course details. Following details will be entered by user and saved in local database (Sqlite database)
Exam/Course name
Number of credits 
Required reference materials
Expected result
Add Assignments

Expected Outcome Success:
New event is created.
The system will create the database and it will save new event in the database.
Expected Outcome Failure:
Event creation process is cancelled. 
Course name does empty
Number of credit does empty
Duplicate course or exam
Valid Input Specification
Input Field
Valid Input
Exam/Course name
Alphanumeric, min 3, max 255
Number of credit
Numeric. Min value 1
Required reference materials 
Alphanumeric, min 2, max 255
Expected Result
Alphanumeric, values  A, B, C 
Assignment Name
Alphanumeric, min 2, max 255
Assignment start and due date
Date format
Table 1 – Form Input Data 
Test Approach
The valid input domain for this feature is too large to manually test all possible values. The input is straight data entry. The functional tests will be designed using equivalence classes defined equivalence class partitioning analysis. The boundary value defined in the following table 03. 
EC
Description
Valid/Invalid
1
Exam/Course name contains all alphanumeric values
Valid
2
Exam/Course name contains non-alphanumeric values
Invalid
3
Exam/Course name has between 3 and 255 alphanumeric characters
Valid
4
Exam/Course name has less than 3 alphanumeric values
Invalid
5
Exam/Course name has more than 255 alphanumeric values
Invalid
6
Number of credit is 1 or more
Valid
7
Number of credit is less than 1
Invalid
8
Required reference material name contains all alphanumeric values
Valid
9
Required reference material name contains non-alphanumeric values
Invalid
10
Required reference material name has between 2 and 255 alphanumeric characters
Valid
11
Required reference material name has less than 2 alphanumeric values
Invalid
12
Required reference material name has more than 255 alphanumeric values
Invalid
13
Expected Result contains three alpha values A,B,C or numeric values
Valid
14
Expected Result contains non-alphanumeric values or A,B,C expect others
Invalid
15
Assignment name contains all alphanumeric values
Valid
16
Assignment name contains non-alphanumeric values
Invalid
17
Assignment name has between 3 and 255 alphanumeric characters
Valid
18
Assignment name has less than 3 alphanumeric values
Invalid
19
Assignment name has more than 255 alphanumeric values
Invalid
Table 2 – Equivalence Class Partitions
Boundary Group
Boundary
Value
Length of Exam/Course name. Value just below the lower bound (BLB) 
1
Length of Exam/Course name. Value on the lower boundary (LB) 
2
Length of Exam/Course name. Value just above the lower boundary (ALB) 
3
Length of Exam/Course name. Value just below the upper bound (BUB) 
254
Length of Exam/Course name. Value on the upper bound (UB) 
255
Length of Exam/Course name. Value just above the upper bound (AUB) 
256
Length of Required reference material name. Value just below the lower bound (BLB) 
1
Length of Required reference material name. Value on the lower boundary (LB) 
2
Length of Required reference material name. Value just above the lower boundary (ALB) 
3
Length of Required reference material name. Value just below the upper bound (BUB) 
254
Length of Required reference material name. Value on the upper bound (UB) 
255
Length of Required reference material name. Value just above the upper bound (AUB) 
256
Length of Assignment name. Value just below the lower bound (BLB) 
1
Length of Assignment name. Value on the lower boundary (LB) 
2
Length of Assignment name. Value just above the lower boundary (ALB) 
3
Length of Assignment name. Value just below the upper bound (BUB) 
254
Length of Assignment name. Value on the upper bound (UB) 
255
Length of Assignment name. Value just above the upper bound (AUB) 
256
Below value of number of credit 
0
At boundary value of number of credit 
1
Just above minimum value of number of credit
2
Table 3 – Boundary Values 
	
5.7.3 Set the Exam/Course start and due date 
Feature Under Test: Set the exam/course start and due date 
Use Case: The user can set the date for existing event. After set the start and due date, the system will create progressing bar to get visual idea about working progress. Starting date can be current date or future date. The Due date must future date. 
Working flow chart
Select the course/ exam icon in course catalog view.
Edit view provides date input fields
After setting the dates, user push set date button 
Dates will save in database
Expected Outcome Success:
Add starting and due dates for event.
Percentage bar creates and displays progress.  
Expected Outcome Failure:
Date adding process is cancelled.
Invalid date format or past date entered. 
Valid Input Specification
Input Field
Valid Input
Exam/Course Start and due Dates
Date format
Month
Numeric. Min Length 1 – Max Length 2. Min Value 1 Max Value 12
Day
Numeric. Min Length 1 – Max Length 2. Min Value 1 Max Value 31
Year
Numeric. Length = 4
Table 4 – Form Input Date 

Test Approach
The valid input domain for this feature is too large to manually test all possible values. The input is straight data entry. The functional tests will be designed using equivalence classes defined equivalence class partitioning analysis. The boundary value defined in the following table 06. 

EC
Description
Valid/Invalid
1
Exam/Course Date format meets yyyy/mm/dd or mm/dd/yyyy specifications
Valid
2
Exam/Course Date does not meet format yyyy/mm/dd or mm/dd/yyyy specifications
Invalid
3
Month contains all numeric values	
Valid
4
Month contains non-numeric values
Invalid
5
Month has 1 or 2 numeric characters
Valid
6
Month has less than 1 numeric values
Invalid
7
Month has more than 2 numeric values
Invalid
8
Month has value between 1 and 12
Valid
9
Month has value less than 1
Invalid
10
Month has value more than 12
Invalid
11
Year contains all numeric values
Valid
12
Year contains non-numeric values
Invalid
13
Year has 4 numeric characters
Valid
14
Year has less than 4 numeric values
Invalid
15
Year has more than 4 numeric values
Invalid
16
Date contains all numeric values
Valid
17
Date contains non-numeric values
Invalid
18
Date has 1 or 2 numeric characters
Valid
19
Date has less than 1 numeric values
Invalid
20
Date has more than 2 numeric values
Invalid
21
Date has value between 1 and 31
Valid
22
Date has value less than 1
Invalid
23
Date has value more than 31
Invalid
Table 5 – Equivalence Class Partitions
Boundary Group
Boundary
Value
Length of month. Value just below the lower bound (BLB) 
0
Length of month. Value on the lower boundary (LB) 
1
Length of month. Value on the upper bound (LB) 
2
Length of month. Value just above the upper bound (ALB) 
3
Below Value of Month 
0
At lower boundary value of Month 
1
Just above minimum value of Month 
2
Below Value of maximum upper value of Month
11
At upper boundary value of Month
12
Just above upper boundary value of Month
13
Length of Year. Value just below the boundary 
3
Length of Year. Value on the boundary
4
Length of Year. Value just above the boundary 
5
Length of Date. Value just below the lower bound (BLB) 
0
Length of Date. Value on the lower boundary (LB) 
1
Length of Date. Value on the upper bound (LB) 
2
Length of Date. Value just above the upper bound (ALB) 
3
Below Value of Date 
0
At lower boundary value of Date 
1
Just above minimum value of Date 
2
Below Value of maximum upper value of Date
30
At upper boundary value of Date
31
Just above upper boundary value of Date
32
Table 6 – Boundary Values 

5.7.4 Set the assignment start and due date
Feature Under Test: Set the assignment start and due date 
Use Case: The user can set the date  for any new assignments in existing event. After set the start and due date, the system will create progressing bar to get visual idea about working progress for assignment. Starting date can be current date or future date. The Due date must future date. 
Working flow chart
Select the course/ exam icon in course catalog view.
Select the assignment
Edit view provides date input fields under selected assignment
After setting the dates, user push set date button 
Dates will save in database
Expected Outcome Success:
Add starting and due dates for assignment.
Percentage bar creates and displays progress.  
Expected Outcome Failure:
Date adding process is cancelled.
Invalid date format or past date entered. 
Valid Input Specification
Input Field
Valid Input
Assignment Start and due Dates
Date format
Month
Numeric. Min Length 1 – Max Length 2. Min Value 1 Max Value 12
Day
Numeric. Min Length 1 – Max Length 2. Min Value 1 Max Value 31
Year
Numeric. Length = 4
Table 7 – Form Input Data 
Test Approach
The valid input domain for this feature is too large to manually test all possible values. The input is straight data entry. The functional tests will be designed using equivalence classes defined equivalence class partitioning analysis. The boundary value defined in the following table 09. 

EC
Description
Valid/Invalid
1
Assignment Date format meets yyyy/mm/dd or mm/dd/yyyy specifications
Valid
2
Assignment Date does not meet format yyyy/mm/dd or mm/dd/yyyy specifications
Invalid
3
Month contains all numeric values	
Valid
4
Month contains non-numeric values
Invalid
5
Month has 1 or 2 numeric characters
Valid
6
Month has less than 1 numeric values
Invalid
7
Month has more than 2 numeric values
Invalid
8
Month has value between 1 and 12
Valid
9
Month has value less than 1
Invalid
10
Month has value more than 12
Invalid
11
Year contains all numeric values
Valid
12
Year contains non-numeric values
Invalid
13
Year has 4 numeric characters
Valid
14
Year has less than 4 numeric values
Invalid
15
Year has more than 4 numeric values
Invalid
16
Date contains all numeric values
Valid
17
Date contains non-numeric values
Invalid
18
Date has 1 or 2 numeric characters
Valid
19
Date has less than 1 numeric values
Invalid
20
Date has more than 2 numeric values
Invalid
21
Date has value between 1 and 31
Valid
22
Date has value less than 1
Invalid
23
Date has value more than 31
Invalid
Table 8 – Equivalence Class Partitions


Boundary Group
Boundary
Value
Length of month. Value just below the lower bound (BLB) 
0
Length of month. Value on the lower boundary (LB) 
1
Length of month. Value on the upper bound (LB) 
2
Length of month. Value just above the upper bound (ALB) 
3
Below Value of Month 
0
At lower boundary value of Month 
1
Just above minimum value of Month 
2
Below Value of maximum upper value of Month
11
At upper boundary value of Month
12
Just above upper boundary value of Month
13
Length of Year. Value just below the boundary 
3
Length of Year. Value on the boundary
4
Length of Year. Value just above the boundary 
5
Length of Date. Value just below the lower bound (BLB) 
0
Length of Date. Value on the lower boundary (LB) 
1
Length of Date. Value on the upper bound (LB) 
2
Length of Date. Value just above the upper bound (ALB) 
3
Below Value of Date 
0
At lower boundary value of Date 
1
Just above minimum value of Date 
2
Below Value of maximum upper value of Date
30
At upper boundary value of Date
31
Just above upper boundary value of Date
32
Table 9 – Boundary Values 

5.7.5 Set the reminder for 1%-100% completion  
Feature Under Test: Set the reminder for 1%-100% completion
Use Case: The user can set reminder as notification to get time reminder. After setting time period, it will equal to 100% working time. User can set any stage level such as 20%, 50%, 75% or 95% between total time periods. 
Working flow chart
Select course/exam form list of view
Select get notification button
Add notification time as a percentage between 1%-100%
Click save button 


Expected Outcome Success:
Display Toast message “Saved notification”
Notification save in database
Expected Outcome Failure:
Display Toast message “Error saving notification”
Invalid percentage
Valid Input Specification
Input Field
Valid Input
Notification level 
Numeric, min 1, max 3, Min Value 1 Max Value 100
Table 10 - Form Input Data
Test Approach
The valid input domain for this feature is too large to manually test all possible values. The input is straight data entry. The functional tests will be designed using equivalence classes defined equivalence class partitioning analysis. The boundary value defined in the following table 12. 
EC
Description
Valid/Invalid
1
Notification contains all numeric values	
Valid
2
Notification contains non-numeric values
Invalid
3
Notification has 1 or 2 or 3 numeric characters
Valid
4
Notification has less than 1 numeric values
Invalid
5
Notification has more than 3 numeric values
Invalid
6
Notification has value between 1 and 100
Valid
7
Notification has value less than 1
Invalid
8
Notification has value more than 100
Invalid
Table 11 – Equivalence Class Partitions



Boundary Group
Boundary
Value
Length of Notification. Value just below the lower bound (BLB) 
0
Length of Notification. Value on the lower boundary (LB) 
1
Length of Notification. Value on the upper bound (LB) 
3
Length of Notification. Value just above the upper bound (ALB) 
4
Below Value of Notification 
0
At lower boundary value of Notification
1
Just above minimum value of Notification 
2
Below Value of maximum upper value of Notification
99
At upper boundary value of Notification
100
Just above upper boundary value of Notification
101
Table 12 – Boundary Values 

5.7.6 Update event
Feature Under Test: Update the existing event
Use Case: The user can update existing event by clicking on course/exam icon in course view catalog view. Edit view provides all existing details about selected item and user can update following details and saved in local database (Sqlite database)
Exam/Course name
Number of credits 
Required reference materials
Start and due dates
Expected result
Add Assignments
Assignment start date and due date

Expected Outcome Success:
Existing event is updated.
The system will update the database and it will save and replaced event in the database.
Expected Outcome Failure:
Event update process is cancelled. 
Course name does empty
Number of credit does empty
Duplicate course or exam
Invalid date

Valid Input Specification
Input Field
Valid Input
Exam/Course name
Alphanumeric, min 3, max 255
Number of credit
Numeric. Min value 1
Course Start and due Dates
Date format
Month
Numeric. Min Length 1 – Max Length 2. Min Value 1 Max Value 12
Day
Numeric. Min Length 1 – Max Length 2. Min Value 1 Max Value 31
Year
Numeric. Length = 4
Required reference materials 
Alphanumeric, min 2, max 255
Expected Result
Alphanumeric, values  A, B, C 
Assignment Name
Alphanumeric, min 2, max 255
Assignment start and due date
Date format
Table 13 – Form Input Data 

Test Approach
The valid input domain for this feature is too large to manually test all possible values. The input is straight data entry. The functional tests will be designed using equivalence classes defined equivalence class partitioning analysis. The boundary value defined in the following table 15. 

EC
Description
Valid/Invalid
1
Exam/Course name contains all alphanumeric values
Valid
2
Exam/Course name contains non-alphanumeric values
Invalid
3
Exam/Course name has between 3 and 255 alphanumeric characters
Valid
4
Exam/Course name has less than 3 alphanumeric values
Invalid
5
Exam/Course name has more than 255 alphanumeric values
Invalid
6
Number of credit is 1 or more
Valid
7
Number of credit is less than 1
Invalid
8
Exam/Course/Assignment Date format meets yyyy/mm/dd or mm/dd/yyyy specifications
Valid
9
Exam/Course/ Assignment Date does not meet format yyyy/mm/dd or mm/dd/yyyy specifications
Invalid
10
Month contains all numeric values	
Valid
11
Month contains non-numeric values
Invalid
12
Month has 1 or 2 numeric characters
Valid
13
Month has less than 1 numeric values
Invalid
14
Month has more than 2 numeric values
Invalid
15
Month has value between 1 and 12
Valid
16
Month has value less than 1
Invalid
17
Month has value more than 12
Invalid
18
Year contains all numeric values
Valid
19
Year contains non-numeric values
Invalid
20
Year has 4 numeric characters
Valid
21
Year has less than 4 numeric values
Invalid
22
Year has more than 4 numeric values
Invalid
23
Date contains all numeric values
Valid
24
Date contains non-numeric values
Invalid
25
Date has 1 or 2 numeric characters
Valid
26
Date has less than 1 numeric values
Invalid
27
Date has more than 2 numeric values
Invalid
28
Date has value between 1 and 31
Valid
29
Date has value less than 1
Invalid
30
Date has value more than 31
Invalid
31
Required reference material name contains all alphanumeric values
Valid
32
Required reference material name contains non-alphanumeric values
Invalid
33
Required reference material name has between 2 and 255 alphanumeric characters
Valid
34
Required reference material name has less than 2 alphanumeric values
Invalid
35
Required reference material name has more than 255 alphanumeric values
Invalid
36
Expected Result contains three alpha values A,B,C or numeric values
Valid
37
Expected Result contains non-alphanumeric values or A,B,C expect others
Invalid
38
Assignment name contains all alphanumeric values
Valid
39
Assignment name contains non-alphanumeric values
Invalid
40
Assignment name has between 3 and 255 alphanumeric characters
Valid
41
Assignment name has less than 3 alphanumeric values
Invalid
42
Assignment name has more than 255 alphanumeric values
Invalid
43
Assignment Date format meets yyyy/mm/dd or mm/dd/yyyy  specifications
Valid
44
Assignment Date format does not meet yyyy/mm/dd or mm/dd/yyyy specifications
Invalid
Table 14 – Equivalence Class Partitions
Boundary Group
Boundary
Value
Length of Exam/Course name. Value just below the lower bound (BLB) 
1
Length of Exam/Course name. Value on the lower boundary (LB) 
2
Length of Exam/Course name. Value just above the lower boundary (ALB) 
3
Length of Exam/Course name. Value just below the upper bound (BUB) 
254
Length of Exam/Course name. Value on the upper bound (UB) 
255
Length of Exam/Course name. Value just above the upper bound (AUB) 
256
Length of Required reference material name. Value just below the lower bound (BLB) 
1
Length of Required reference material name. Value on the lower boundary (LB) 
2
Length of Required reference material name. Value just above the lower boundary (ALB) 
3
Length of Required reference material name. Value just below the upper bound (BUB) 
254
Length of Required reference material name. Value on the upper bound (UB) 
255
Length of Required reference material name. Value just above the upper bound (AUB) 
256
Length of Assignment name. Value just below the lower bound (BLB) 
1
Length of Assignment name. Value on the lower boundary (LB) 
2
Length of Assignment name. Value just above the lower boundary (ALB) 
3
Length of Assignment name. Value just below the upper bound (BUB) 
254
Length of Assignment name. Value on the upper bound (UB) 
255
Length of Assignment name. Value just above the upper bound (AUB) 
256
Length of month. Value just below the lower bound (BLB) 
0
Length of month. Value on the lower boundary (LB) 
1
Length of month. Value on the upper bound (LB) 
2
Length of month. Value just above the upper bound (ALB) 
3
Below Value of Month 
0
At lower boundary value of Month 
1
Just above minimum value of Month 
2
Below Value of maximum upper value of Month
11
At upper boundary value of Month
12
Just above upper boundary value of Month
13
Length of Year. Value just below the boundary 
3
Length of Year. Value on the boundary
4
Length of Year. Value just above the boundary 
5
Length of Date. Value just below the lower bound (BLB) 
0
Length of Date. Value on the lower boundary (LB) 
1
Length of Date. Value on the upper bound (LB) 
2
Length of Date. Value just above the upper bound (ALB) 
3
Below Value of Date 
0
At lower boundary value of Date 
1
Just above minimum value of Date 
2
Below Value of maximum upper value of Date
30
At upper boundary value of Date
31
Just above upper boundary value of Date
32
Below value of number of credit 
0
At boundary value of number of credit 
1
Just above minimum value of number of credit
2
Table 15 – Boundary Values 

5.7.7 Delete event
Feature Under Test: Delete event
Use Case: The user can delete course/exam from course catalog view. There is delete button in the action bar menu in the application. 
Working flow chart
Select the event that user needs to delete
Click the delete button 

Expected Outcome Success:
The toast message displayed “Event deleted”
The event completely delete from database and this event can’t recover. 
Expected Outcome Failure:
User event was not deleted. 
User does not select event. 
Valid Input Specification
Event select from event list in course catalog view.\
Test Approach
The input domain for this test case is small and dependent on several business logic specifications. The tests are designed starting with a decision table. The following table, Table 16, contains the decision table for this test case.
Conditions
Select status 


Event 
True
False
Actions




Delete 
True
False
Table 16 – Decision table for delete test



Pass/fail criteria
If under certain situations defects in the application or products can happen and it results errors in the causing failure.  Not all defects results failures since some of them stay as inactive. Defects in dead code will never result in failures. The failures assign a level of severity. Severity gives an idea about how the failure influence on system’s function and customer satisfaction. Following severity levels gives different output.
Severity level 1 and 2 – catastrophic; system can’t be operated. So, testing will stop and the product is not released.
Severity level 3 and 4- minimal effect on the user of the software. Testing can be continued to release the product.
Suspension and resumption criteria
Testing of software is usually perform in regular business hours, from Monday to Friday. During these hours all defects are discovered and severity of defects are rated and logged into a document. If testing severity is in level 1 or 2 or hardware failure occurs, the testing will be suspended.
Test deliverables
Core sets of deliverable are required for any software testing phase. Some deliverables are provided before testing phase, some during the testing phase and the others after the testing cycle. The following are the list of test deliverables.
Test Specifications document
Test Plan document
Test Strategy
Test Scenarios document
Test Design standards
Test Case document
Traceability matrix
Test execution reports
Test logs
Bug reports
Test summary reports
Test Data
Flow document
Test Metrics
Test Status reports

Testing Tasks
Testing is the process of analyzing a software item to detect the differences between existing and required conditions and to evaluate the features of the software item.  Testing tasks are developed by the product manager, software team lead and the team. The list of testing tasks includes:
Preparing a test plan
Preparing test design specifications
Preparing test case reproduction steps
Supervising the test team
Execution of functional tests and recording results
Update of existing test plans
Connecting product testing to real-time
Attending daily stand-up meetings
Tracking different metrics
Ensuring that all testers have access to test tools and documentation
Distributing the test summary reports

Testing environment
Lab setup- There are different Android emulators in Android studio, based on Ubuntu 14.04 Operating system. Also, there is a Git version control system and we will use master branch, development branch and testing branch. When we complete the testing, we will merge it to the master branch. Also, there is a log management system that will use to identify activities. 
Publications- All test documentation including user cases, acceptance tests and test cases are stored in the source control system and providing all the testers access to the testing tools and documentation. Any other necessary documentation will be provided, according to tester’s requirement.
Responsibilities
We are a small team including product owner, 2 developers and two non-developers. According to their skills and given tasks, responsibilities are spread within the team. The product owner and developers are responsible for developing the testing strategy, test cases and track the product performance. Non-developers will follow the test cases specification and do documentation.
Anuruddha Pathirana- Product owner/test manager
Owen Martin- lead developer/tester
Alex Cook- developer/tester
Wayne Tanner- non-developer/tester
Saman Perera- non-developer/tester



Staff and training needs
Testing of the software is performed by above mentioned team. Only existing hardware and software will be used. Monthly meetings are arranging to discuss the progress of the development and testing. Also, the lead developer, Owen Martin will conduct training sessions for non-developers in two weeks before the test.
Scheduling
The duration of the task and schedule is described in detail in the following table.

Risks and contingencies
Since the test team is quite small, there are only few members to identify the defects of the software and fix it. The rest will have only the basic understanding of the test plan. 
Approval
Test manager, Project manager and Software quality assurance manager will approve the test plan to be completed.
…………………………………………………
James Weaver			Date
Test Manager

…………………………………………………
Susan Jennings			Date
Project Manager


……………………………………………………
Michael Smith       	          Date
SQA Manager

References 

Burnstein, I. (2003). Practical software testing: A process-oriented approach. New York, NY: Springer – Verlag.
