# ADFR001 Test Strategy

The aim of this document is to describe a simple and robust Test Strategy for project *<Project Name>*. It includes or references the guidance and standards that will inform:

1. Code reviews 
2. Software design decisions at all levels
3. The technical stack used for Test Frameworks
4. The level of quality assurance within the software delivery lifecycle (SDLC)

## **Version Control**

This is a living document that will evolve over the lifecycle of any project. It must be contained within the project repository and version controlled accordingly (using Git). The first draft of this document must be agreed before any project commences. 

## **Ownership**

This document will be owned and maintained by Development, with assistance and independent oversight from the Test Team.

## **High Level Test Strategy**

The table below describes the types of testing that must be performed during the Agile SDLC:

| Name               | Manual / Automated | Description |
|--------------------|--------------------|-------------|
| [Unit Testing](Unit Testing.md) | Automated | Tests for individual units of code. Any interfaces or dependences are mocked.|
| Functional Testing | Automated | Tests to ensure that the logic coded into the application fulfils the user requirements. These are currently called 'Integration Tests' or 'Deep Tests'.|
| E2E Testing | Automated | Tests to exercise the entire application stack. Typically run from the application UI and mimic user interaction. |
| Visual Testing | Automated | Tests to ensure that the visual elements of the application are correct. This is not tested by E2E or functional tests. |
| Exploratory Testing | Manual | Tests to ensure that unexpected user activity does not result in unhandled application failure. |

Each of these Test Types has a dedicated section within this document below.

The table below describes how these types of testing integrate with a typical Agile SDLC:

| SDLC Phase            | Test Process                                                      |
|-----------------------|-------------------------------------------------------------------|
| Sprint Planning       | BDD Scenarios created                                             |
| During the Sprint     | Unit Tests, Functional Tests and E2E Tests completed (Automated). |
| Outside of the Sprint | Exploratory Testing performed (Manual)                            |

## **Continuous Integration**

Describe here when the different automated regression tests are run in the CI pipeline. E.g.

| Action                  | Regression Testing Performed                                                            |
|-------------------------|-----------------------------------------------------------------------------------------|
| Push to Branch          | All Functional Tests and Visual Tests are run for that Feature.                         |
| Merge to Release Branch | All Functional Tests run for all Features, all E2E tests run, all Visual Tests are run. |

## **Defect Management**

With the exception of Exploratory Testing, all issues with the code identified by failing tests will be corrected within the Sprint and not documented as defects.
