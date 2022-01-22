# SENG 438 - Software Testing, Reliability, and Quality
# Lab Report \#1 – Introduction to Testing and Defect Tracking

| Group \#:       | 25 |
|-----------------|----|
| Curtis Silva    |    |
| Divyansh Goyal  |    |
| Gurpartap Sohi  |    |
| Liam Parmar     |    |

<hr>

**Table of Contents**

(When you finish writing, update the following list using right click, then
“Update Field”)

[1 Introduction](#introduction)

[2 High-Level Plan for Exploratory Testing](#high-level-plan-for-exploratory-testing)
* [2.1 Introduction](#introduction-1)
* [2.2 High Level Functions and Descriptions](#high-level-functions-and-descriptions)
* [2.3 Testing Approach](#testing-approach)
* [2.4 Test Creation Process](#test-creation-process)
* [2.5 Justification of Test Plan](#justification-of-test-plan)

[3 Comparison of exploratory and manual functional testing](#comparison-of-exploratory-and-manual-functional-testing)

[4 Notes and discussion of the peer reviews of defect reports](#)

[5 How the pair testing was managed and team work/effort was
divided](#_Toc439194681)

[6 Difficulties encountered, challenges overcome, and lessons
learned](#_Toc439194682)

[7 Comments/feedback on the lab and lab document itself](#_Toc439194683)

<hr>

## Introduction

This assignment intends to provide students a generalized overview of various types of software testing including exploratory testing, manual scripted testing, and regression testing. In order to perform exploratory testing, students are required to devise a high level plan to test features of an ATM Simulation System extensively and report defects that are determined during the tests. In order to perform the manual scripted testing, students will execute the predetermined test cases sequentially and report any defects. Regression testing will be performed with the updated version of the ATM Simulation System using the test cases that produced defects in the earlier tests and observing whether the previously present defects have been resolved. Prior to this lab, members of the group had a combined understanding that the difference between exploratory and manual functional testing is that exploratory testing is the creation of spontaneous tests while executing tests, while manual functional testing is when there is a predefined set of tests and only those tests are executed. The group believed that the method which is more effective in determining bugs is manual functional testing due to its structural format of fixed tests spanning all functionalities.

<hr>

## High-Level Plan for Exploratory Testing
### Introduction
The following test plan is designed to perform spontaneous, exploratory tests on the ATM Simulation System version 1.0. The intention of these tests is to test all the claimed features in the Requirements section of the ATM Simulation System documentation. The plan will identify the test determination procedures, the tasks performed by each member of the team, the general timeline, and the procedures for reporting observed defects.

### High Level Functions and Descriptions
| <strong>High Level Function</strong>       | <strong>Description</strong> |
|-----------------|----|
| Turning system on  | The user should be able to successfully turn the system on, only when the system is currently in the off state.   |
| Validation of User PIN    | Displays a message when the PIN entered by the user is invalid for the card number associated with it.   |
| Deposit     | A user can make a deposit to a checking, savings, or money market account. Once the type of account is selected, the ATM system will then prompt the user to enter a positive deposit amount. After pressing enter, a button which represents the user inserting a deposit envelope appears.   |
| Withdrawal  | A user must be able to withdraw a multiple of $20 from any account provided the account contains enough funds within it.   |
| Balance inquiry | A user may have one or more accounts and can only see the balance of those accounts that are associated with the card number. |
| Transferring between accounts | A user can make a transfer of money between any two accounts linked to the card inputted into the ATM. |
| Receipt | The ATM will provide the user with a receipt after every successful transaction. The receipt will contain information regarding the time, date, location, transaction type, accounts involved, amount, and available balances of the affected accounts. |
| Timeout | If a user does not input an envelope in a specified time duration when making a deposit in the account, a timeout occurs. |
| Turning system off | The user should be able to successfully shut the system off only when the system is currently in the “on” state. |

### Testing Approach
The testing approach the testers decided to implement consists of splitting up the group of four into pairs consisting of two members each, where one member of the pair will record defects and bugs on Backlog and the other member will run the executable and implement the tests. Both members of each pair will contribute in determining and running tests. Each pair will perform testing and recording defects on Backlog for approximately half an hour. During the exploratory testing, each pair will test every high-level function and will focus more on functions where more test cases can be implemented. The functions which contain more specifications and steps involved in the process, such as transferring, depositing, and withdrawing will be given more importance during the testing process compared to the other high level functions. One group will focus more on deposits and transfers, whereas the other group will focus more on withdrawals.

### Test Creation Process
To create tests spontaneously, each pair will first begin with testing features and inputs that theoretically should not cause any errors/bugs. For example, when withdrawing money, the first test will be to withdraw $20 as that requirement is present in the ATM specifications, implying that this condition will be met by the system. Following these tests, each pair will discuss and determine inputs which may potentially cause an error in the system, such as inputting a value which is not a multiple of $20 for withdrawing money, and observing the system’s response. If errors persist, the pair will continue testing similar inputs and try to replicate the error to determine the overall range of the inputs causing errors.

### Justification of Test Plan
By splitting into pairs, one member can record defects into Backlog while simultaneously brainstorming with the other member regarding tests to run on the ATM Simulation System, thus increasing productivity. Furthermore, by having two teams testing on the same system, not only will there be rigorous testing of each functionality, but there will also be different focuses which will provide a deeper-level understanding of areas causing bugs or errors within each sub-system. By dividing areas of focus, there is a reduction in the chance of overlapping test cases, which will provide a greater variety of errors identified. By testing inputs which have a higher chance of generating successful outputs first, testers can narrow inputs down to the more problematic ones by gaining a deeper understanding of what works and what doesn’t. Exploratory testing provides a benefit due to its adaptable nature, where the tester can intuitively focus on specific problematic areas rather than an even distribution provided by scripted tests.

<hr>

## Comparison of exploratory and manual functional testing

Text…

-   Note that you need to submit a report generated by your defect tracking
    system, containing all defects recorded in the system.
    
<hr>

## Notes and discussion of the peer reviews of defect reports

Text…

<hr>

## How the pair testing was managed and team work/effort was divided 

Text…

<hr>

## Difficulties encountered, challenges overcome, and lessons learned

Text…

<hr>

## Comments/feedback on the lab and lab document itself

Text…
