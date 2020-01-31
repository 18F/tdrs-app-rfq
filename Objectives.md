# Objectives

## Backlog

The set of preliminary user stories set forth below will be the starting
point for the development of software to be provided under this
contract. These preliminary user stories are provided only for
illustrative purposes, and do not comprise the full scope or detail of
the project. OFA expects that the Contractor will work closely with the
Product Owner to perform regular user research and usability testing and
to develop and prioritize a full gamut of user stories as the project
progresses.

Individual user stories may be modified, added, retracted, or
reprioritized by the Product Owner at any time, in coordination with the
Contractor's team. OFA expects that the user stories will be
continuously refined during the development process.

-   As a data and reporting specialist, I need clear data validation, so
    I have confidence that errors are being found and flagged as early
    as possible.

-   As a data and reporting specialist, I need customizable data
    validation rules, so I can adapt my validation rules as my program
    requires.

-   As a data and reporting specialist, I need all my data in one
    database so I can create custom queries.

-   As a data and reporting specialist, I need plain-language guidance
    on how to enter my data and how to remedy data input errors, so I
    understand the process I am required to follow.

-   As a data and reporting specialist, I need the ability to append
    metadata to my reports, so I can flag issues I'm having or why I
    have chosen to leave some fields blank.

-   As a data and reporting specialist, I need automated and timely
    messages that confirm my data has been received, so I know I have
    met my reporting requirements.

-   As a data and reporting specialist, I need basic data visualization
    capabilities, so I can spend less time manually building reports.

-   As a data and reporting specialist, I need a reporting system that
    accepts multiple file formats, so I do not manually have to enter
    data into an interface.

-   As a program director, I need an easy-to-use interface, so that
    staff of varying capacity levels and comfort with technology will
    be able to successfully use the system.

-   As a program director, I need different levels of access for
    different types of users, so that personally identifiable
    information (PII) is kept confidential.

-   As a program director, I need a data reporting format that meets
    Congressional reporting requirements.

## List of Deliverables with Quality Assurance Surveilance Plan (QASP)

The following chart sets forth the performance standards and quality
levels the code and documentation provided by the Contractor must meet,
and the methods OFA will use to assess the standard and quality levels
of that code and documentation.

Deliverable          | Performance Standard(s) | Acceptable Quality Level | Method of Assessment | Due Date
---------------------|-------------------------|--------------------------|----------------------|---------
Tested Code          | Code delivered under the order must have substantial test code coverage.
Version-controlled [Agency] GitHub repository of code that comprises product that will remain in the government domain. | Minimum of 90% test coverage of all code. All areas of code are meaningfully tested. | Combination of manual review and automated testing | Every sprint
Properly Styled Code | [GSA 18F Front- End Guide](https://frontend.18f.gov/#js-style) | 0 linting errors and 0 warnings | Combination of manual review and automated testing | Every sprint
Accessible           | Web Content Accessibility Guidelines 2.1 AA standards | 0 errors reported using an automated scanner and 0 errors reported in manual testing | https://github.com/pa11y/pa11y | 
Deployed             | Code must successfully build and deploy into staging environment. | Successful build with a single command | Combination of manual review and automated testing | Every sprint
Documented           | All dependencies are listed and the licenses are documented. Major functionality in the software/source code is documented. Individual methods are documented inline in a format that permit the use of tools such as JSDoc. System diagram is provided. | Combination of manual review and automated testing, if available | Manual review | Every sprint
Secure               | OWASP Application Security Verification Standard 3.0 | Code submitted must be free of medium- and high-level static and dynamic security vulnerabilities | Clean tests from a static testing SaaS (such as Snyk or npm audit) and from OWASP ZAP, along with documentation explaining any false positives | Every sprint
User research        | Usability testing and other user research methods must be conducted at regular intervals throughout the development process (not just at the beginning or end). | Research plans and artifacts from usability testing and/or other research methods with end users are available at the end of every applicable sprint, in accordance with the contractor’s research plan. | OFA will manually evaluate the artifacts based on a research plan provided by the contractor at the end of the second sprint and every applicable sprint thereafter. | As needed
