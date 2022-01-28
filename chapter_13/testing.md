# Testing

Testing is an important part of developing software.

In your project, you will be required to test your project, along with
documenting your testing objectives, processes, and strategies within
Confluence.

This will introduce the different types of testing to students and
explain how to write a test plan.

## Why Write Tests?

Software testing is the process of verifying that the software you have
developed meets the requirements of the client.

The benefits of testing include:

-   Identify bugs in your software.
-   Identify regression failures (checking if new code breaks existing
    features).
-   Reduce reliance on developers to test different cases.
-   Automate tests is much faster than running test scenarios by hand.

## Types of Testing

Each type of testing will be discussed in further detail below.

| Type                | Description                                                                                                               |
|---------------------|---------------------------------------------------------------------------------------------------------------------------|
| Unit testing        | Checking whether each software unit performs as expected. The finest level of granularity in testing.                     |
| Integration testing | Checking whether multiple software components/units operate correctly.                                                    |
| Acceptance testing  | Checking whether the application meets the client's requirements. Acceptance tests are created based on the user stories. |

### Unit Testing

Unit testing is completed during the development of an application and
is completed by the developers. When a developer picks up a task from
the task tracking tool, they are expected to implement the task as
required and prove that the unit of work does what they say it does.
This is where unit testing comes in.

Unit tests isolate a section of code to verify correctness. A unit may
be an individual function, method, procedure, module, or object.

#### Reasons to Complete Unit Testing

1.  Unit tests help to fix bugs early in the development cycle when it
    is less expensive and easier to locate bugs.
2.  Good unit tests serve as project documentation.
3.  Unit tests permit code re-use - if you know a component you have
    created is thoroughly tested and works well, you can introduce it
    into other parts of your application's codebase without being
    concerned it will cause issues.

There is a tension that exists in software testing between available
time to implement a task and time that should be spent on testing each
task. Many developers cut down on testing time to complete more work.
This is a myth that you can somehow minimise time spent testing and end
up with a fully functional and bug-free piece of software.

It in fact saves time unit testing tasks as they are completed. They are
easy to isolate - introducing a buggy component into a larger piece of
work is akin to finding a needle in a haystack when bugs arise later
(and bugs will arise later, if you have not tested them).

#### Types of Unit Testing

There are two primary types of unit testing: manual and automated.

##### Manual Unit Testing

As the name suggests, this involves manually testing a unit of work.
This is normally done by the developer who completed the work and
involves creating documentation detailing the step-by-step instructions
(with screenshots and comments) showing the success scenarios of the
unit, as well as any failure scenarios.

This documentation should be tested and confirmed by a reviewer (another
member of the development team).

##### Automated Unit Testing

There are several tools that can be used to automate unit testing
(depending on the language chosen for your project). Some examples are:

1.  [JUnit](https://junit.org/junit5/): a popular and free
    testing tool for Java.
2.  [Jest](https://jestjs.io): a popular and free testing
    tool for JavaScript.
3.  [Testing library](https://testing-library.com/).
4.  [Mocha](https://mochajs.org): a popular and free
    testing tool for JavaScript.

### Integration Testing

Integration testing involves integrating software modules and testing
them as a group.

You might wonder why integration testing is necessary when all tasks
have (hopefully) been unit tested:

1.  A unit is designed by one developer whose understanding and
    programming logic may differ from other developers. Integration
    testing verifies that software modules work in unity regardless of
    which developer developed the module.
2.  Changes of requirements by the clients could mean some modules are
    outdated and need to be tested and integrated carefully.
3.  Calls and return statements between software modules and the
    database, hosting service, etc. could be erroneous.
4.  Exception handling between components could be lacking.

Integration testing differs from other tests as it primarily focuses on
information and data flow between modules. The emphasis is on
integrating links between modules.

As an example, you might have two modules:

1.  Authentication component
2.  Email component.

Both modules work as expected when conducting unit testing, but now the
team must test that information flows from authentication to the email
module. An example test case might be:

| Test Case ID | Objective                                                   | Description                                         | Expected Result                                             |
|--------------|-------------------------------------------------------------|-----------------------------------------------------|-------------------------------------------------------------|
| 1            | Test the link between the authentication and email modules. | Enter login and credentials and click login button. | User should be successfully redirected to the email module. |


This is just one example of testing the integration between two
components - when conducting actual integration testing, there would
likely be many more tests.

#### Automated Integration Testing

There are several tools that can be used to automate integration testing
(depending on the language chosen for your project). Some examples are:

1. [Playwright](https://playwright.dev/)
2. [Cypress](https://www.cypress.io/)

### Acceptance Testing

Acceptance testing tests whether the system meets the requirements as
specified by the client - it tests whether the system passes or fails a
given user story.

Often, the process of acceptance testing begins during the requirements
phase. Teams write acceptance criteria to describe a pass/fail set of
criteria that is used to determine whether a user story is completed.
Acceptance criteria do not care about how you implement the
functionality.

Once you have your acceptance criteria, you can use this to write test
cases that are used to verify the result of the criteria (acceptance
tests).

#### Acceptance Criteria Template

When writing acceptance criteria, you should use the template below:

Given that \[condition\], when \[something happens\], then \[result\].

#### Acceptance Criteria Vs. Acceptance Tests

| Acceptance Criteria                           | Acceptance Test                                 |
|-----------------------------------------------|-------------------------------------------------|
| Measures if a user story is completed.        | Verifies if the product works for users.        |
| Written before implementation.                | Written during development.                     |
| Describes what areas to cover in the project. | Uses criteria to test key areas of the project. |

As an example, here is a list of the acceptance criteria for a project
from semester 2, 2021:

![](resources/acceptance_criteria.png)

You can see in the screenshot above that the acceptance criteria links
to: epic, user story, and details the criteria for a pass result.

This criterion was then test using acceptance tests and the results were
manually captured in screenshots and added to the Confluence page:

![](resources/acceptance_testing.png)

The details in the acceptance test (screenshots + steps involved) allow
the tests to be easily reproduced by the development team, client, or
academic staff in the future.

```{note}

- Your team should have 1-3 acceptance criteria per user story.
- Acceptance criteria are written before implementation.
- They are independently testable.
- They have a defined pass or fail result.

```

### Visualising Testing

The hierarchy of testing can be visualised as:

![](resources/testing_hierarchy.svg)

## Test Plan

Test plans document the team's testing strategy, objectives, tools, and
processes for the project.

Testing plans are important as they ensure:

-   All team members understand the objectives the team must strive to
    achieve.
-   Ensures testing is not neglected throughout the project.
-   Forces the team to think about how they will verify the quality of
    their product.

### What to Include in a Test Plan?

-   Testing objectives.
-   Testing tools/frameworks.
-   In scope/Out of scope (what aspects of the system will/won't be
    tested).
-   A clear description of what types of testing will be completed.
    Should provide detail as to who will be conducting the testing and
    when testing will occur.
-   Bug reporting strategy (when a bug is identified, what process
    should the team follow?).

You can view a very thorough example of a test plan [here](https://www.softwaretestinghelp.com/test-plan-sample-softwaretesting-and-quality-assurance-templates/).

## Code Coverage

A common metric for thoroughness of your test plan is code coverage. It
examines what proportion of code is covered by a test. While code
coverage is not an indicator of success (i.e., coverage scores of 100%
does not necessarily mean you have tested the right things), it is a
good indicator of test extensiveness. Code coverage score greater than
80% is generally considered sufficient.

Code coverage works by testing many or all the below:

1.  *Function coverage:* how many of the functions defined have been
    called.
2.  *Statement coverage:* how many of the statements in the program have
    been executed.
3.  *Branches coverage:* how many of the branches of the control
    structures (if statements for instance) have been executed.
4.  *Condition coverage:* how many of the Boolean sub-expressions have
    been tested for a true and a false value.
5.  *Line coverage:* how many of lines of source code have been tested.

Code coverage reports are created in the process by tools (detailed
below) and are displayed:

![](resources/code_coverage.png)

*Source*: [Atlassian](https://www.atlassian.com/continuous-delivery/software-testing/code-coverage)

### Automating Code Coverage

There are many tools that can automate code coverage, but the two most
popular are:

1. [Cypress](https://docs.cypress.io/guides/tooling/code-coverage#Introduction).
2. [Istanbul](https://github.com/gotwarlost/istanbul).
