# BDD (Behaviour-Driven Development)

## Aim

Behaviour-Driven Development ensures that the system is designed around the functional requirements of the user. It also ensures functional issues are identified as early as possible, typically when the business logic is created.

## Guidance

The following simple process will be followed for any User Story. 

Please note: the BDD process below doesn't include the CI or Code Control quality processes (e.g. code reviews).

| Step # | Step                                                | Owner                | Output                                                                                                                               |
|--------|-----------------------------------------------------|----------------------|--------------------------------------------------------------------------------------------------------------------------------------|
| BDD01  | A Feature File is created containing the User Story | Product Owner        | Feature File containing the User Story.                                                                                              |
| BDD02  | An Example Mapping session is held                  | Product Owner        | Acceptance Criteria added to Feature File                                                                                            |
| BDD03  | Scenarios are created                               | Developer and Tester | Scenarios added to Feature file                                                                                                      |
| BDD04  | Scenarios are reviewed by Product Owner             | Product Owner        | Updated scenarios (if necessary)                                                                                                     |
| BDD05  | Technical implementation discussion                 | Developers           | Technical implementation notes are captured and E2E scenarios are identified.                                                        |
| BDD06  | Scenarios are implemented in the code               | Developers           | Functional Tests covering all scenarios are created and test report is green. Unit Tests have been created and test report is green. |
| BDD07  | Any E2E test scenarios are implemented              | Developer / Tester   | E2E tests. E2E test report is green.                                                                                                 |

### **Functional Testing**

Functional Testing will be performed to ensure that all user requirements have been met by the functionality of the system.

*A description of the Technical Stack of the Functional Test framework and a brief description as to how it is implemented must be included here to support the developers.*

| Tool  | Description | Use |
|-------|-------------|-----|
| Karma | Test Runner |     |
| TBC   |             |     |

### **E2E Tests**

End to end tests will be identified during the Technical Review (step BDD05 of the BDD process) by the following criteria:

1. The middleware API is triggered
2. The scenario covers business functionality that is provided by Guidewire or the middleware. 
3. The scenario is High Risk or High Impact

*A description of the Technical Stack of the E2E Test framework must be included here to support the developers and Testers.*

| Tool  | Description | Use |
|-------|-------------|-----|
| Protractor | Test Automation Framework |     |
| TBC   |             |     |

## Continuous Improvement

There is currently no cross-browser testing performed. It may be more effective to do this with any Visual Testing framework that is created (see next section). If cross-browser testing is performed with the E2E framework, then it may be useful to mock any middle tier and network responses, to maximise the speed and reliability of these tests.

There is currently no integration into the CI environment or any 'tagging' strategy for scenarios.
