# Software Testing

## Famous software failures
### Wrong approach
- Reserve more time for testing at the end of the development? 
- Write more test cases?
- Spend more money on testing?

### Right approach
- Do testing throughout the development process 
- Write better test cases 
- Spend cost-effective money on testing (e.g., improve testability) 

## Terminology
| Term | Description |
| --- | ----------- |
| Software failure | A component or a software system behaves in a way that is not expected. |
| Software defect (or bug or fault): | A flaw in a component or in any part of the software that causes the system to behave incorrectly. |
| Error (or mistake): | It is about the human action that produces the incorrect result. |
| Software Validation | Making sure that our system delivers what the user needs it to deliver. (are we building the right the system?) |
| Software Verification: | Making sure that our system delivers what the specification wants it to deliver, that it is free of bugs. (are we building the system right?) |
| Error | An Error indicates serious problem that a reasonable application should not try to catch. Exception: Exception indicates conditions that a reasonable application might try to catch. |
| Exceptions | An exception is an not wanted event during the execution of your code which interrupts your program at runtime. |

## Test Automation
The use of software to control the execution of tests, the comparison of actual outcomes to predicted outcomes, the setting up of test preconditions, and other test control and test reporting functions.

### Benefits
- Reduces costs
- Reduces human error
- Reduces variance in test quality from different individuals
- Reduces the cost of regression testing


### Software Testability
The degree to which a system or component facilitates the establishment of test criteria and the performance of tests to determine whether those criteria have been met.

Dominated by two problems
• How hard is it to **provide the test values** to the software
• How hard is it to **observe the results** of test execution

| Controllability      | Observability |
| ----------- | ----------- |
| How easy it is to provide a program with the needed inputs, in terms of values, operations, and behaviors. Input from hardware sensors or distributed software is harder to provide | How easy it is to observe the behavior of a program in terms of its outputs, effects on the environment and other hardware and software components Software that affects hardware devices, databases, or remote files have low observability |

## Components of a Test Case
A test case is a multipart artifact with a definite structure

| Component | Description |
| --- | ----------- |
| Test case values | The input values needed to complete an execution of the software under test [“Tim”] |
| Expected results | The result that will be produced by the test if the software behaves as expected (“Student”) |
| Test oracle | It uses the expected results to decide whether a test passed or failed |
| Prefix values | Input necessary to put the software into the state to receive the test case values |
| Postfix values | Input need to be sent to the software after the test case values are sent |
| Test case | The test case values, prefix values, postfix values, and expected results necessary for execution and evaluation |
| Test set/suite | A set of test cases |
| Test script | A test case that is prepared in a form to be executed automatically on the tested software and produce a report |
| Prefix values | A set of assumptions, concepts, and tools that support test automation |



```markdown
[Link](url) and ![Image](src)
```

