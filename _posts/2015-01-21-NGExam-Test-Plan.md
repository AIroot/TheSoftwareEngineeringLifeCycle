---
layout: post
title: Software Test Plan Outline
---

### NGE Mobile Application Test Plan

### Anuruddha I Jayasekara Pathiranage

01/21/2015

### Table of Contents

1.0
TEST PLAN IDENTIFIER………………………………………………………...3

2.0
INTRODUCTION………………………………………………………………….3

2.1
NATURE OF THE PROJECT………………………………………………3

2.2
SYSTEM TEST OBJECTIVES AND SCOPE……………………………..4

2.2.1
Test Objectives………………………………………………………4

2.2.2
Testing Scope………………………………………………………..4

2.3
RELATED DOCUMENTS………………………………………………….5

3.0
ITEMS TO BE TESTED…………………………………………………………...5

4.0
FEATURES…………………………………………………………………………5

4.1
FEATURES TO BE TESTED……………………………………………….5

4.2
FEATURES NOT TO BE TESTED…………………………………………5

5.0
APPROACH………………………………………………………………………..6

5.1
SOURCES OF SAMPLE……………………………………………………6

5.2
TESTING TEAM……………………………………………………………6

5.3
RECORD DOCUMENTING FOR TEST………………………………….6

5.4
TEST STATUS………………………………………………………………6

5.5
TEST TOOLS……………………………………………………………….7

5.6
STOP TEST CRITERIA…………………………………………………….7

5.7
TEST CASES……………………………………………………………….7

5.7.1
USER GUIDE LINE………………………………………………..7

5.7.2
CREATE NEW EVENT……………………………………………..8

5.7.3
SET THE EXAM/COURSE START AND DUE DATE……………11

5.7.4
SET THE ASSIGNMENT START AND DUE DATE……………..13

5.7.5
SET THE REMAINDER OF 1% -100% COMPLETION………….16

5.7.6
UPDATE EVENT……………………………………………………18

5.7.7
DELETE EVENT……………………………………………………22

6.0
PASS/FAIL CRITERIA……………………………………………………….........23

7.0
SUSPENSION AND RESUMPTION CRITERIA………………………….……...24

8.0
TEST DELIVERABLES……………………………………………………….......24

9.0
TESTING TASKS………..………………………………………………………...25

10.0
TESTING ENVIRONMENT……………………………………………………...26

11.0
RESPONSIBILITIES……………………………………………………………...26

12.0
STAFF AND TRAINING NEEDS………………………………………………...27

13.0
SCHEDULING…………..………………………………………………………...27

14.0
RISKS AND CONTINGENCIES………………………………………………...27

15.0
APPROVAL………………………………………………………………………...27

REFERENCE………………………………………………………........................28


### Test Plan Recognizer

QANGE001


### 2.0 Introduction

This section introduces the mobile application under test, providing basic background information, an overview, test objectives and scope. There is a list of related documents attached.
2.1 Nature of the Project

NGE is a mobile based Android mobile application to organize exam and courses in universities and any educational institutes for students and exam takers. This can  be used as an online or offline application based on user’s android device. NGE provides easy and well organized pre-design content for exam and courses. Users can create events for their exam and they can assign their target achievement as a grade or percentage of point. Then application provides guide lines to achieve their target in unique way according to the user. 

There is a notification system and progressing bar to indicate future action and past work for user. When user creates exam or course event, system will create local database and table for new event. After creating the event, user can notify what are the important things that have to focus those areas in exam or course. This notification works with time frame. The application provides multi task facility and if there are any past activities, those activities will use as past experiences to predict new event’ achievement. This function is more helpful to get a big motivation for success in event. 

### 2.2 Application Test Objectives and Scope

This test plan describes the application requirement, environment, activities, tasks, tools, costs, and schedules for system testing the NGE application.

	### 2.2.1 Test Objectives

The objectives for application system testing are to validate the following sections:

01. Create and organize exam and course event
02. Notification based user activity

The test objectives are:

01. Ensure full functional areas act in accordance with each exam and courses with related institute.

02. The application is user friendly and easy to use.

03. The application meets its performance requirements.

04. The application can handle crash reporting and exception.

05. User experience and user interface with different devices. 


	### 2.2.2 Test Scope

The project will test the version 1.0 release of the new application and will perform set of application tests including:

Functional Testing- Creation new course event, verification of real time progressing bar, viewing available event, notification system, input data validation, verification of past data identification with current event

Performance Testing – Event saving time, event delete time

Reliability Testing – Accuracy of data entry, completed records

	### 2.3 Related Documents

		1. User privacy agreement

		2. Input data specification

### 3.0 Items To Be Tested

	1. Application user’s guide line modules

	2. Event creation modules

	3. Real time notification modules

	4. Completed event handling modules


### 4.0 Features

	### 4.1 Features To Be Tested
		### Create and organize exam and course event
			
			1. User guide line

			2. Create new event

			3. Update event

			4. Delete event


	### Notification based user activity

			1. Set the Assignment due date 

			2. Set the course due date

			3. Set the reminder for 50%, 75%, 95% competence 

	### 4.2 Features Not To Be Tested

The Android operating system’s SQLITE database is not tested under this plan. This application run on Android API 15-24. This API compatibility in not tested in this plan. 


### 5.0 Approach

The NGE Android mobile development team does not have a separate testing group. Testing also should be done by mobile developer in the team. They have the necessary resources and a test environment to support their test effort. In the mobile application all items will be tested until requirements are satisfied and to ensure the software will work properly. There is well organized document handle system which save all test cause, specification for future testing.

### 5.1 Sources of Sample

The team will create dummy event as a user using virtual courses and exam due dates.

### 5.2 Testing team

The one main developer for NGE will be responsible for test case design, test execution, and the recording of test results. Other developer will provide assistance as needed. 

### 5.3 Record documenting for test

All test results will be recorded in a test log file and saved on the test file directory. All test failures will be captured in a problem report and given a severity grade level. 

### 5.4 Test Status

There is no automated test. The status of the test event will be reported and discussed with team. 

### 5.5 Test Tools

The following tools will be used to do test easier. Any tester has good training to use the tools. The tools are the following:

	* Android Emulator

	* Git version control system

### 5.6 Stop-Test Criteria

Stop testing is depend on defect level. The decision to stop the testing will be based on how many defects are discovered versus how many requirements are covered.

### 5.7 Test Cases

### 5.7.1 User guide line

#### Feature Under Test: User Guide Line

#### Use Case: A new user can get idea about how to use the application to organizing their courses and exam. 

#### Working flow chart

1. Install the NGE app into the device. 

2. Click the app icon in the device

3. When the app open first UI display User guide lines step by step.

#### Expected Outcome Success:

Display the user guide line.

* Guide line can be scrollable and clear to understand 

* Guide line provides complete details about how to use the application

#### Expected Outcome Failure: 
				
Guide line is not displayed

* Application view Error

#### Test Approach

Course catalog view is the main user interface that will show the course as list view. If there is an empty view (without any courses) it will display user guidelines.  There is an action bar that has delete icon to delete courses and past experiences icon to collect finished exams or courses. Finished courses can highlight to collect into the past experiences. Also Fab button will link to the edit view.

There is no valid input domain. The guide line creates and displays as a system default option. If the guide line is not displayed there is system error. 

### 5.7.2 Create new event

#### Feature Under Test: 

Create new event

#### Use Case:

The user can add or edit courses into the app database using Course catalog view by pressing fab button or on courses icon.  Then it will open edit view to get course details. Following details will be entered by user and saved in local database (Sqlite database)

* Exam/Course name

* Number of credits 
			
* Required reference materials

* Expected result

* Add Assignments

#### Expected Outcome Success:

New event is created.

The system will create the database and it will save new event in the database.

#### Expected Outcome Failure:

Event creation process is cancelled. 

1. Course name does empty

2. Number of credit does empty

3. Duplicate course or exam

#### Valid Input Specification

Table 1 – Form Input Data 

#### Test Approach

The valid input domain for this feature is too large to manually test all possible values. The input is straight data entry. The functional tests will be designed using equivalence classes defined equivalence class partitioning analysis. The boundary value defined in the following table 03. 


Table 2 – Equivalence Class Partitions



Table 3 – Boundary Values 
	
### 5.7.3 Set the Exam/Course start and due date 

#### Feature Under Test: 

Set the exam/course start and due date 

#### Use Case: 

The user can set the date for existing event. After set the start and due date, the system will create progressing bar to get visual idea about working progress. Starting date can be current date or future date. The Due date must future date. 

#### Working flow chart

* Select the course/ exam icon in course catalog view.

* Edit view provides date input fields

* After setting the dates, user push set date button 

* Dates will save in database


#### Expected Outcome Success:

Add starting and due dates for event.

* Percentage bar creates and displays progress.  

#### Expected Outcome Failure:

Date adding process is cancelled.

* Invalid date format or past date entered. 

#### Valid Input Specification

Table 4 – Form Input Date 


#### Test Approach

The valid input domain for this feature is too large to manually test all possible values. The input is straight data entry. The functional tests will be designed using equivalence classes defined equivalence class partitioning analysis. The boundary value defined in the following table 06. 


Table 5 – Equivalence Class Partitions

Table 6 – Boundary Values 

### 5.7.4 Set the assignment start and due date

#### Feature Under Test: 

Set the assignment start and due date 

#### Use Case: 

The user can set the date  for any new assignments in existing event. After set the start and due date, the system will create progressing bar to get visual idea about working progress for assignment. Starting date can be current date or future date. The Due date must future date. 

#### Working flow chart

1. Select the course/ exam icon in course catalog view.

2. Select the assignment

3. Edit view provides date input fields under selected assignment

4. After setting the dates, user push set date button 

5. Dates will save in database

#### Expected Outcome Success:

Add starting and due dates for assignment.

* Percentage bar creates and displays progress.  

#### Expected Outcome Failure:

Date adding process is cancelled.

* Invalid date format or past date entered. 

#### Valid Input Specification

Table 7 – Form Input Data 

#### Test Approach

The valid input domain for this feature is too large to manually test all possible values. The input is straight data entry. The functional tests will be designed using equivalence classes defined equivalence class partitioning analysis. The boundary value defined in the following table 09. 



Table 8 – Equivalence Class Partitions


Table 9 – Boundary Values 

### 5.7.5 Set the reminder for 1%-100% completion 

#### Feature Under Test: 

Set the reminder for 1%-100% completion

#### Use Case: 

The user can set reminder as notification to get time reminder. After setting time period, it will equal to 100% working time. User can set any stage level such as 20%, 50%, 75% or 95% between total time periods. 

#### Working flow chart

1. Select course/exam form list of view

2. Select get notification button

3. Add notification time as a percentage between 1%-100%

4. Click save button 


#### Expected Outcome Success:

Display Toast message “Saved notification”

* Notification save in database

#### Expected Outcome Failure:

Display Toast message “Error saving notification”

* Invalid percentage

#### Valid Input Specification

Table 10 - Form Input Data

#### Test Approach

The valid input domain for this feature is too large to manually test all possible values. The input is straight data entry. The functional tests will be designed using equivalence classes defined equivalence class partitioning analysis. The boundary value defined in the following table 12. 


Table 11 – Equivalence Class Partitions

Table 12 – Boundary Values 

### 5.7.6 Update event

#### Feature Under Test: 

Update the existing event

#### Use Case: 

The user can update existing event by clicking on course/exam icon in course view catalog view. Edit view provides all existing details about selected item and user can update following details and saved in local database (Sqlite database)

* Exam/Course name

* Number of credits 

* Required reference materials

* Start and due dates

* Expected result

* Add Assignments

* Assignment start date and due date

#### Expected Outcome Success:

Existing event is updated.

The system will update the database and it will save and replaced event in the database.

#### Expected Outcome Failure:

Event update process is cancelled. 

1. Course name does empty

2. Number of credit does empty

3. Duplicate course or exam

4. Invalid date

#### Valid Input Specification

Table 13 – Form Input Data 

#### Test Approach

The valid input domain for this feature is too large to manually test all possible values. The input is straight data entry. The functional tests will be designed using equivalence classes defined equivalence class partitioning analysis. The boundary value defined in the following table 15. 

Table 14 – Equivalence Class Partitions

Table 15 – Boundary Values 

### 5.7.7 Delete event

#### Feature Under Test: 

Delete event

#### Use Case: 

The user can delete course/exam from course catalog view. There is delete button in the action bar menu in the application. 

#### Working flow chart

* Select the event that user needs to delete

* Click the delete button 

#### Expected Outcome Success:

The toast message displayed “Event deleted”
The event completely delete from database and this event can’t recover. 

#### Expected Outcome Failure:

User event was not deleted. 

* User does not select event. 

#### Valid Input Specification

Event select from event list in course catalog view.


#### Test Approach

The input domain for this test case is small and dependent on several business logic specifications. The tests are designed starting with a decision table. The following table, Table 16, contains the decision table for this test case.

Table 16 – Decision table for delete test


### 6.0 Pass/fail criteria

If under certain situations defects in the application or products can happen and it results errors in the causing failure.  Not all defects results failures since some of them stay as inactive. Defects in dead code will never result in failures. The failures assign a level of severity. Severity gives an idea about how the failure influence on system’s function and customer satisfaction. Following severity levels gives different output.

Severity level 1 and 2 – catastrophic; system can’t be operated. So, testing will stop and the product is not released.

Severity level 3 and 4- minimal effect on the user of the software. Testing can be continued to release the product.


### 7.0 Suspension and resumption criteria

Testing of software is usually perform in regular business hours, from Monday to Friday. During these hours all defects are discovered and severity of defects are rated and logged into a document. If testing severity is in level 1 or 2 or hardware failure occurs, the testing will be suspended.

### 8.0 Test deliverables

Core sets of deliverable are required for any software testing phase. Some deliverables are provided before testing phase, some during the testing phase and the others after the testing cycle. The following are the list of test deliverables.

* Test Specifications document

* Test Plan document

* Test Strategy

* Test Scenarios document

* Test Design standards

* Test Case document

* Traceability matrix

* Test execution reports

* Test logs

* Bug reports

* Test summary reports

* Test Data

* Flow document

* Test Metrics

* Test Status reports

### 9.0 Testing Tasks

Testing is the process of analyzing a software item to detect the differences between existing and required conditions and to evaluate the features of the software item.  Testing tasks are developed by the product manager, software team lead and the team. The list of testing tasks includes:

* Preparing a test plan

* Preparing test design specifications

* Preparing test case reproduction steps

* Supervising the test team

* Execution of functional tests and recording results

* Update of existing test plans

* Connecting product testing to real-time

* Attending daily stand-up meetings

* Tracking different metrics

* Ensuring that all testers have access to test tools and documentation

* Distributing the test summary reports

### 10.0 Testing environment

Lab setup- 
There are different Android emulators in Android studio, based on Ubuntu 14.04 Operating system. Also, there is a Git version control system and we will use master branch, development branch and testing branch. When we complete the testing, we will merge it to the master branch. Also, there is a log management system that will use to identify activities. 
Publications- All test documentation including user cases, acceptance tests and test cases are stored in the source control system and providing all the testers access to the testing tools and documentation. Any other necessary documentation will be provided, according to tester’s requirement.

### 11.0 Responsibilities

We are a small team including product owner, 2 developers and two non-developers. According to their skills and given tasks, responsibilities are spread within the team. The product owner and developers are responsible for developing the testing strategy, test cases and track the product performance. Non-developers will follow the test cases specification and do documentation.

* Anuruddha Pathirana- Product owner/test manager

* Owen Martin- lead developer/tester

* Alex Cook- developer/tester

* Wayne Tanner- non-developer/tester

* Saman Perera- non-developer/tester



### 12.0 Staff and training needs

Testing of the software is performed by above mentioned team. Only existing hardware and software will be used. Monthly meetings are arranging to discuss the progress of the development and testing. Also, the lead developer, Owen Martin will conduct training sessions for non-developers in two weeks before the test.

### 13.0 Scheduling

The duration of the task and schedule is described in detail in the following table.

### 14.0 Risks and contingencies

Since the test team is quite small, there are only few members to identify the defects of the software and fix it. The rest will have only the basic understanding of the test plan. 

### 15.0 Approval

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


### References 

Burnstein, I. (2003). Practical software testing: A process-oriented approach. New York, NY: Springer – Verlag.
