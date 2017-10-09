---
layout: post
title: Software Quality Assurance, Testing Fundamentals and Analysis 
---

### Test Case Analysis: Equivalence Classes

### [Equivalence Class Testing](https://github.com/AIroot/common-assets/blob/master/pdf/EquivalenceClassTesting.pdf)

Equivalence class theory is proposed by Glenford Myers. Equivalent Class Partitioning is a black box technique that can be applied to all levels of testing such as unit, integration, system, etc. It attempts to reduce the total number of test cases necessary by partitioning the input conditions into equivalence classes. The principal of equivalence class testing is formation of equivalence classes. In this method, input or output data is grouped into sets of data that behave in a same way using an Equivalence relation.(Gupta, n.d.) In this method we consider both valid and invalid input domains. An equivalence relation describes how data is going to be processed when it enters a function. In order to get the full potential of the equivalence class testing, some time should be spent on designing a strong equivalence relation. Creating a strong equivalence relation will result in optimal and useful test cases.(“LU-raksti-751.pdf,” n.d.) 

### Test Case Analysis: Boundary Values

### [Boundary Value Testing](https://github.com/AIroot/common-assets/blob/master/pdf/Boundary%20Value%20Testing.pdf)

Any program needs inputs and gives outputs from its range. This input and output can be considered as a function. The Boundary value analysis is the best technique to use for functional testing. The goal of functional testing is to use knowledge of the basic function of a program to identify test cases. The Boundary Value Testing focuses on the boundary of the input space to identify test cases. The reasoning behind boundary value testing is that errors tend to occur near the extreme values of an input variable.(Basili & Selby, 1987) 

The basic idea in boundary value is to select input variable value at their:

* Minimum

* Just above the minimum

* A nominal value

* Just below the maximum

* Maximum


### Test Case Analysis: Decision Tables

### [Decision table testing](https://github.com/AIroot/common-assets/blob/master/pdf/Decision%20Tables%20Testing.pdf)

A decision table is an outstanding technique used in both testing and requirements management. It is a structured exercise to prepare requirements when dealing with complex business rules. Decision Table Testing is useful to deal with a combination of inputs, which produce different results. It helps reduce test effort in verifying each and every combinations of test data, at the same time ensuring complete coverage. Decision tables are very much helpful for testers to search the effects of combinations of different inputs and other software states that must correctly implement business rules(Chilenski & Miller, 1994). 



### Test Case Analysis: Pairwise Testing

### [Pairwise Testing](https://github.com/AIroot/common-assets/blob/master/pdf/Pairwise%20Testing.pdf)

Pairwise testing has become an indispensable tool in a software tester’s toolbox. The technique has been known for almost 20 years (Tai & Lei, 2002),  but only last five years there has a tremendous increase in its popularity. Pairwise testing is a wildly popular approach for combinatorial testing problems. Pairwise testing is an economical alternative tool to testing all possible combinations of a set of variables. In pairwise testing a set of test cases is generated that covers all combinations of the selected test data values for each pair of variables. Pairwise testing is also referred to as all pairs testing and 2-way testing. Also we can do all triples (3-way) or all quadruples (4- way) testing, of course, but the size of the higher order test sets grows very rapidly.  Generally, pairwise testing begins by selecting values for the system’s input variables. These individual values are often selected using domain partitioning. The values are then permuted to achieve coverage of all the pairings(Bach & Schroeder, 2004).


### Test Case Analysis: State-Transitions

### [State-Transition Testing](https://github.com/AIroot/common-assets/blob/master/pdf/StateTransitionTesting.pdf)

State-Transition diagrams are excellent tools to capture certain types of system requirements and to document internal system design. State Transition testing, a black box testing technique, in which outputs are triggered by changes to the input conditions or changes to 'state' of the system. This is based on finite state machine(Chow, 1978). In general, a state machine is any device that stores the status of something at a given time and can operate on input to change the status and/or cause an action or output to take place for any given change. A computer is basically a state machine and each machine instruction is input that changes one or more states and may cause other actions to take place.  In other words, tests are designed to execute valid and invalid state transitions(tutorialspoint.com, n.d.).


### Test Case Analysis: Control Flow

### [Control Flow Testing](https://github.com/AIroot/common-assets/blob/master/pdf/ControlFlowTesting.pdf)

In structural testing, the software is viewed as a white box and test cases are determined from the implementation of the software. Control-flow testing is a structural testing strategy that uses the program’s control flow as a model and this can use the control structure of a program to develop the test cases for the program. The control structure of a program can be represented by the control flow graph of the program. Flow graphs consist of three primitives.

01. A decision is a program point at which the control can diverge.

02. A junction is a program point where the control flow can merge.

03. A process block is a sequence of program statements uninterrupted by either decisions or junctions (Naik & Tripathy, 2008).

There are three testing criteria for control flow testing.

* Path Testing: Execute all possible control flow paths through the program.

* Statement Testing: Execute all statements in a program at least once under some test.

* Branch Testing: Execute enough tests to assure that every branch alternative has been exercised at least once under some test (Ostrand, 2002).


### [Project Component: Test Plan Outline](https://github.com/AIroot/TheSoftwareEngineeringLifeCycle/blob/master/assets/pdf/NGExamTestPlan.pdf)

### [Project Component: Agile Story Cards & Acceptance Criteria](https://github.com/AIroot/TheSoftwareEngineeringLifeCycle/blob/master/assets/pdf/Agile%20Story%20Cards%20and%20Acceptance%20Criteria.pdf)

### [Project Component: Formal Test Cases](https://github.com/AIroot/TheSoftwareEngineeringLifeCycle/blob/master/assets/pdf/FormalTestCases.pdf)






