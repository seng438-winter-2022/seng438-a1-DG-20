# SENG 438 - Software Testing, Reliability, and Quality
# Lab Report \#1 – Introduction to Testing and Defect Tracking

| Group \#:       | 25 |
|-----------------| -- |
| Curtis Silva    |    |
| Divyansh Goyal  |    |
| Gurpartap Sohi  |    |
| Liam Parmar     |    |

<hr>

**Table of Contents**

[1 Introduction](#introduction)

[2 High-Level Plan for Exploratory Testing](#high-level-plan-for-exploratory-testing)
* [2.1 Introduction](#introduction-1)
* [2.2 High Level Functions and Descriptions](#high-level-functions-and-descriptions)
* [2.3 Testing Approach](#testing-approach)
* [2.4 Test Creation Process](#test-creation-process)
* [2.5 Justification of Test Plan](#justification-of-test-plan)

[3 Insights on Comparisons Between Exploratory Testing and Manual Functional Testing](#insights-on-comparisons-between-exploratory-testing-and-manual-functional-testing)

[4 Notes on The Peer Review Process and Reporting Defects as A Group](#notes-on-the-peer-review-process-and-reporting-defects-as-a-group)

[5 Pair Testing Management and Division of Responsibilities](#pair-testing-management-and-division-of-responsibilities)

[6 Lessons Learned from Teamwork](#lessons-learned-from-teamwork)

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
The testing approach the testers decided to implement consists of splitting up the group of four into pairs consisting of two members each, where one member of the pair will record defects and bugs on Backlog and the other member will run the executable and implement the tests. Both members of each pair will contribute in determining and running tests. Each pair will perform testing and recording defects on Backlog for approximately half an hour. During the exploratory testing, each pair will test every high-level function and will focus more on functions where more test cases can be implemented. The functions which contain more specifications and steps involved in the process, such as transferring, depositing, and withdrawing will be given more importance during the testing process compared to the other high level functions. One group will focus more on deposits and balance inquiries, whereas the other group will focus more on withdrawals and transfers.

### Test Creation Process
To create tests spontaneously, each pair will first begin with testing features and inputs that theoretically should not cause any errors/bugs. For example, when withdrawing money, the first test will be to withdraw $20 as that requirement is present in the ATM specifications, implying that this condition will be met by the system. Following these tests, each pair will discuss and determine inputs which may potentially cause an error in the system, such as inputting a value which is not a multiple of $20 for withdrawing money, and observing the system’s response. If errors persist, the pair will continue testing similar inputs and try to replicate the error to determine the overall range of the inputs causing errors.

### Justification of Test Plan
By splitting into pairs, one member can record defects into Backlog while simultaneously brainstorming with the other member regarding tests to run on the ATM Simulation System, thus increasing productivity. Furthermore, by having two teams testing on the same system, not only will there be rigorous testing of each functionality, but there will also be different focuses which will provide a deeper-level understanding of areas causing bugs or errors within each sub-system. By dividing areas of focus, there is a reduction in the chance of overlapping test cases, which will provide a greater variety of errors identified. By testing inputs which have a higher chance of generating successful outputs first, testers can narrow inputs down to the more problematic ones by gaining a deeper understanding of what works and what doesn’t. Exploratory testing provides a benefit due to its adaptable nature, where the tester can intuitively focus on specific problematic areas rather than an even distribution provided by scripted tests.

<hr>

## Insights on Comparisons Between Exploratory Testing and Manual Functional Testing
The ATM Simulation System was thoroughly tested using both exploratory testing and manual functional testing using a given test suite. Although there are advantages and disadvantages to both types of testing, in this particular system, it was determined that the type of testing method which identified more bugs/errors, and thus was more effective, was exploratory testing. Through the exploratory testing process, 20 unique bugs were identified, whereas through the manual functional testing, only five bugs were discovered, of which only two were undiscovered in the exploratory tests. 

The benefit of the exploratory testing process, which was prevalent when testing this system, was that once an issue was discovered, testers were able to further perform tests on the same function. This allowed testers to determine more bugs in each function, and record them in more detail as understanding of causes of bugs increased through extensive testing. As such, exploratory testing was determined to be far less restrictive than manual functional testing which allowed the testers to determine where to focus upon. Exploratory testing contained a tradeoff between efficiency and thoroughness. Since testers wanted to be thorough once a bug was discovered, more detailed tests needed to be formulated spontaneously, which took time, and thus reduced efficiency.

Manual functional testing provided an advantage in efficiency. Since the 40 tests were pre-defined, testers did not have to spend any time in determining test cases, unlike in exploratory testing, which significantly decreased the time spent on testing. Furthermore, in the given test suite, expected outputs were clearly described, and thus testers were not required to spend more time in formulating the expected outputs to compare against the actual outputs. As such, manual functional testing was much faster and much more efficient. Manual functional contained a tradeoff in the opposite direction as exploratory testing; efficiency against detailed functionality testing. Since the given test suite contained few tests for each function, and had a rigid structure prohibiting testers to further explore areas of concern, there were much fewer bugs identified. However, the whole process contained no time spent on formulation of tests, and thus was much more efficient.

    
<hr>

## Notes on The Peer Review Process and Reporting Defects as A Group
The peer review was conducted by each pair coming together to discuss their recorded bug results after executing the exploratory testing plan. When discussing, the first pair began by reporting the defects they encountered for a certain high level requirement, which was followed by the second pair discussing the defects they found for the same requirement. This process was carried out for each high level requirement. The first pair, who focused more on testing deposits and balance inquiries of the ATM system, discovered and documented 11 defects. Specifically one receipt defect, four deposit defects, one withdrawal defect, three balance inquiry defects, one transfer defect, and one session defect. The second pair, who focused more on testing withdrawals and transfer transactions, discovered and documented 9 defects. The second group recorded four withdrawal defects, one deposit defect, two balance inquiry defects, and two transfer defects. In reviewing defects found for all high level requirements, the pairs were able to catch similar defects and determine whether they were unique in nature. One withdrawal defect, two balance inquiry defects, and one transfer defect were determined to be duplicates for a total of 4 duplicate defects. The group then reported each defect to the backlog software and decided to report one of the duplicate defects as a regular defect, and marked the other with a “[DUPLICATE]” tag in the title.

<hr>

## Pair Testing Management and Division of Responsibilities
The detailed plan for pair testing and the division of focus on high level requirements is explored in detail in the section [2.3](#testing-approach). According to the plan, the pairing was made so that one pair consisted of Divyansh and Curtis, and the other pair consisted of Liam and Gurpartap. Each pair divided the work of exploratory testing amongst themselves with one member performing the driving of the testing using the jar file while sharing their screen and the other keeping track of the discovered defects, in detail. Before commencing testing, the group discussed which of the ATM Simulation System’s high-level requirements to focus on more, in order to avoid overlapping. This was done to make the exploratory testing more efficient among the group and provide greater insight into defective areas of the system.

<hr>

## Lessons Learned from Teamwork
Working extensively in a team to thoroughly test the provided ATM Simulation System allowed the group to gain a lot of insight. One of the biggest lessons provided by this exercise was that the creation of a clear and organized plan/strategy and division of responsibilities ensures that all group members are aware of their roles and this creates a more cohesive team. A well-defined plan also allows the team to work efficiently as every member has the same objective and knows all of the steps needed to achieve that objective. This was evident in the exploratory testing process as both pairs did not discover many duplicate bugs. Furthermore, teamwork allows processes to be completed much faster as different individuals perform different tasks simultaneously, which greatly decreases the operation time. An example of this was when the group divided tasks during the regression testing phase. Here, one individual of the group was running the tests on the ATM Simulation System, another was reading out the steps to reproduce each recorded bug and the input required to recreate it, another group member was creating new defect reports for newly discovered bugs, and finally the last group member was marking the current defects as “in-progress” or “resolved” according to feedback received from the member testing on the system. Through these lessons learned, the importance of teamwork and proper communication became very evident.

<hr>

## Difficulties encountered, challenges overcome, and lessons learned

Text…

<hr>

## Comments/feedback on the lab and lab document itself

Text…
