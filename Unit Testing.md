# Unit Testing

## Aim

Unit Tests are the only way code can be monitored against breaking changes (mutations) in the code. 

However, they can also be used to document the design of the code, eliminating the need to capture and maintain this information elsewhere.

The guidance below covers both uses.

## Guidance

### **Code Design**

*The application will be built of standard components that perform different functions (for example, the MVC (Model, View, Controller) design model). The design should be captured here at a high level.*

*Templated or example Unit Tests should be linked to within this document and describe each of the typical components of the software design. They should describe the mocks, stubs and spies that can be used with them. Example assertions on the logic, structure and data should be included.*

*If this is not possible, or exceptions are needed, this should be captured here, along with a strategy to standardise the design in the future.*

*These templates should be used to enforce good code design, inform code reviews and enable TDD (Test-Driven Development) if the developer uses this methodology.*

### **Test Framework**

*A description of the Technical Stack of the Unit Test framework and a brief description of how it is implemented must be included here to support the developers.*

| Tool  | Description | Use |
|-------|-------------|-----|
| Karma | Test Runner |     |
| TBC   |             |     |

## **Coverage and Reporting**

Test coverage is currently measured through Karma and can be used to inform Code Reviews to ensure that a developer is writing unit tests. 

## Continuous Improvement

| Improvement                        | Detail                                                                                                                                                                                                                                                                                                                                                    | Owner | Status |
|------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------|--------|
| Test Coverage to be included in CI | Test coverage will be included in SonarQube and CI. However it is emphasised that this must not be used as an indicator of code quality in isolation. Ideally this will be used to inform Development of their own quality processes, and not reported throughout the business as it can be easily mis-interpreted.                                       |       |        |
| Mutation Testing                   | Mutation testing needs to be included in the CI pipeline. A PoC needs to be created to identify how best this can be used where best to include it in the Agile SDLC. Again, this will inform the Development team of the effectiveness of their quality processes, and is usually only shared with stakeholders who can correctly interpret the results. |       |        |
