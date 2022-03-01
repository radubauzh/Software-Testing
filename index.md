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

## Junit

- Open source Java testing framework used to write and run repeatable automated tests JUnit is open source (junit.org)
- A structure for writing test drivers
- JUnit features include:
  -  Assertions for testing expected results
  -  Test features for sharing common test data
  -  Test suites for easily organizing and running tests o Graphical and textual test runners
- JUnit is widely used in industry
- JUnit can be used as stand alone Java programs (from the command line) or within an IDE such as Visual Studio Code

## Structure
- JUnit can be used to test ... 
  - an entire object
  - parts of an object (a method or some interacting methods) 
  - the interaction between several objects 
- It is primarily intended for unit and integration testing, not system testing
- Each test case is embedded into one test method
- A test class contains one or more test methods 
- Test classes include : 
  - A collection of test methods
  - Methods to set up the state before and update the state after each test and before and after all the tests 


## Writing tests
- Need to use the methods of the junit.framework.assert class 
  - javadoc gives a complete description of its capabilities
- Each test method checks a condition (assertion) and reports to the test runner whether the test failed or succeeded
- The test runner uses the result to report to the user (in command line mode) or update the display (in an IDE)
- All of the methods return void 
- A few representative methods of junit.framework.assert: 
  - assertTrue (boolean) 
  - assertTrue (String, boolean) 
  - fail (String) 

## IV (Test fixture) 
- A test fixture is the state of the test 
  - Objects and variables that are used by more than one test 
  - Initializations (prefix values)
  - Reset values (postfix values) 
- Different tests can use the objects without sharing the state Objects used in test fixtures are declared as instance variables 
- They should be initialized in a @Before method [example: create list]
- Can be deallocated or reset in an @After method [“Tim”, “Max”]

## Data-Driven Tests 
- Problem: Testing a function multiple times with similar values 
  - How to avoid test code bloat? 
- Simple example: Adding two numbers 
  - adding a given pair of numbers is just like adding any other pair 
  - You really only want to write one test 
-	Data-driven unit tests call a constructor for each set of test values 
  - Same tests are then run on each set of data values 
  - Collection of data values defined by method tagged with @Parameters annotation 

## Data-Driven Tests - Theories 
- Unit tests can have actual parameters 
  - So far, we’ve only seen parameterless test methods 

- Contract model: Assume, Act, Assert 
  - Assumptions (preconditions) limit values appropriately 
  - Action performs activity under scrutiny
  - Assertions (postconditions) check result 











```markdown
[Link](url) and ![Image](src)
```

