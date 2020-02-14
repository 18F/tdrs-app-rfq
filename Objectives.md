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

| Deliverable | Performance Standard(s) | Acceptable Quality Level | Method of Assessment |
| --- | --- | --- | --- |
| Tested Code | Code delivered under the order must have substantial test code coverage. Version-controlled CMS GitHub repository of code that comprises product that will remain in the government domain. | Minimum of 90% test coverage of all code measured by [Codecov](https://codecov.io/). All areas of code are meaningfully tested. | Combination of manual review and automated testing |
| Properly Styled Code | [Airbnb Style Guide](https://github.com/airbnb/javascript) and [prettier](https://prettier.io/) for Javascript. CSS and Sass conforms to Block-Element-Modifier [BEM](http://getbem.com/) | 0 linting errors and 0 warnings | Combination of manual review and automated testing with eslint |
| Accessible | Web Content Accessibility Guidelines 2.1 AA (WCAG 2.1 AA) standards | 0 errors reported for WCAG 2.1 AA standards using an automated scanner and 0 errors reported in manual testing | [http://squizlabs.github.io/HTML\_CodeSniffer/](http://squizlabs.github.io/HTML_CodeSniffer/) or [https://github.com/pa11y/pa11y](https://github.com/pa11y/pa11y) |
| Deployed | Code must successfully build and deploy into staging environment. | Successful build with a single command | Combination of manual review and automated testing |
| Documentation | All dependencies are listed and the licenses are documented. Major functionality in the software/source code is documented. Individual methods are documented inline using comments that permit the use tools such as JsDoc. System diagram is provided. | Combination of manual review and automated testing, if available | Manual review |
| Secure | OWASP Application Security Verification Standard 3.0 | Code submitted must be free of medium- and high-level static and dynamic security vulnerabilities | Clean tests from a static testing SaaS (such as Snyk or npm audit) and from OWASP ZAP, along with documentation explaining any false positives |
| User Research | Usability testing and other user research methods must be conducted at regular intervals throughout the development process (not just at the beginning or end). | Research plans and artifacts from usability testing and/or other research methods with end users are available at the end of every applicable sprint, in accordance with the contractor’s research plan. | OFA will manually evaluate the artifacts based on a research plan provided by the contractor at the end of the second sprint and every applicable sprint thereafter. |

## Environment

### System Requirements

The System must incorporate an intuitive web-based interface that is accessible from both internal and external platforms, including desktops, laptops, tablets, thin/zero clients, and mobile devices. The System architecture must incorporate Application Programming Interfaces (APIs) to intermediate major components. The System must not have a single point of failure. The System will use elastic, dynamically-allocated computing resources that accommodate changing demand in real time. The System must include Login.gov user authentication and authorization functionality and use open source encryption protocols. 

At some point in the future, the system may migrate to an ACF cloud environment. The type of environment is unknown at this time, so the application should be written to be as operationally portable as possible.


### Software Requirements

The software architecture must be extensible to allow for future development. The code base must incorporate analytics, monitoring, continuous integration, and measurement tools. Application design and development must use [plain language](https://content-guide.18f.gov/plain-language/) to the extent practical.

### Design Requirements

Any website that is developed or otherwise delivered as a result of this contract shall be in compliance with the website standards of the Technology Transformation Services of the General Services Administration.
The U.S. Web Design System (USWDS) shall be adopted incrementally over the life of the requirement and the contractor shall prioritize implementation to align with the priorities identified within the SOO. 

### Environments

The System will be hosted on Cloud.gov (a FedRAMP-certified internet-connected Platform as a Service). OFA will own and manage the Cloud.gov account and create development, staging, and production environments for this project within that account. The Contractor will have access to the development environment and will be responsible for maintaining that environment. The Contractor must post all developed code to a public source repository (such as GitHub) designated by OFA. OFA will be responsible for creating and managing this repository. OFA will be responsible for setting up and maintaining a Continuous Integration/Continuous Deployment system to automate the deployment of the code in GitHub. OFA will be responsible for creating, maintaining, and managing the Login.gov integrations.

### System Access

All contractor personnel working under the resulting contract will need to obtain a Homeland Security Presidential Directive 12 [HSPD-12](https://www.dhs.gov/homeland-security-presidential-directive-12) low risk security clearance (or moderate risk security clearance if handling PII) and may need to obtain a personal identity verification (PIV) card in order to perform legacy system integration work. See section 9.9 for additional details.

Contractor personnel that are required to obtain a PIV card will be issued a government-furnished laptop from OFA. Any work that requires access to and handling of PII must be performed on the OFA government-furnished laptop. Contractor personnel that are not required to obtain a PIV card can use contractor-furnished equipment to perform work.

Contractors may have to establish multi-factor authentication (MFA) to access systems which would require government laptops with PIV cards or only MFA through various applications. 

### Additional info that will be provided TBD

## Personnel Skills and Knowledge

### Key Personnel

The contractor must designate a Facilitator,
Technical Lead, and Design Lead as Key Personnel for this project.

- The Facilitator will be a direct liaison to the government product team, and will be responsible for the supervision and management of all of the contractor’s personnel. The Facilitator does not need to be a separate individual and may be a role also fulfilled by any of the Key Personnel proposed. This person should have a background as a scrum master, product manager, agile coach, or a similar type of role.
- The Technical Lead must have a full understanding of the technical approach to be used by the contractor’s development team and will be responsible for ensuring that the contractor’s development team follows that approach. This person should have a background as an engineer.
- The Design Lead must have a full understanding of the research approach and design patterns to be used by the contractor’s development team and will be responsible for ensuring that the contractor’s development team follows that approach. This person should have a background as an user experience researcher or designer.

### Key Personnel Substitution

Key Personnel substitutions must be
submitted to the CO in writing, and will only be justified in the event
of sudden illness, death, change of employment, or termination of
employment for cause. Contractor requests for a substitution of Key
Personnel must include a detailed explanation of the justifying
circumstances, and a complete résumé for the proposed substitute or
addition, including skills, experience, training, and security clearance
level (if applicable). The CO's failure to approve a proposed
substitution will not constitute grounds for non-performance by the
contractor, or form a valid basis for any claim for money or any
equitable adjustment.

### Skills

The contractor must provide a cross functional team that is
experienced in working in an Agile process. They must be comfortable
delivering value iteratively and able to pivot quickly based on a
continuous learning environment. The contractor team will use prototypes
and working software as tools to test hypotheses and validate
assumptions. The team should be expected to deliver working software
early in the post-award period, and to iteratively improve the software
through ongoing development sprints (2 week intervals).

The relevant skills for this project *may* include---
-   Product management
-   Back-end engineering
-   Front-end engineering
-   DevSecOps engineering
-   User research
-   Content design
-   Visual design
-   User support, training, and onboarding
