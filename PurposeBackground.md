# Purpose and Background

## Purpose

In fiscal year 2020, the Office of Family Assistance (OFA) within the
Administration for Children and Families (ACF) entered into an
interagency agreement with 18F within the Technology Transformation
Service (TTS) to provide assisted acquisition services for the
procurement of software development services in support of the TANF Data
Reporting System (TDRS). OFA is seeking a contractor to assist with TDRS
improvements and enhancements. 18F will award and administer the
resultant contract on behalf of OFA. 18F will provide procurement and
technical support to OFA for the life of the contract.

## Background

The General Services Administration's (GSA) Technology Transformation
Services (TTS) applies modern methodologies and technologies to improve
the public's experience with Government by helping agencies make their
services more accessible, efficient, effective, and by providing
services that exemplify these values.

The Office of Family Assistance (OFA) has entered into an interagency
agreement (IAA) with TTS for assisted acquisition services. TTS will
acquire the services requested in this solicitation on behalf of OFA and
administer the contract in post award.

The Office of Family Assistance (OFA) within the Administration for
Children and Families (ACF) administers the Temporary Assistance for
Needy Families (TANF) program on behalf of the Department of Health and
Human Services (HHS). Since 1996, the TANF program has served as one of
the nation's primary economic security and stability programs for
low-income families with children. TANF is a block grant that provides
\$16.6 billion annually to states, territories, the District of
Columbia, and federally-recognized Indian tribes. These TANF
jurisdictions use federal TANF funds to provide income support as well
as a wide range of services to vulnerable families with minor children.

As part of oversight and administration of the TANF Program, OFA
operates the TANF Data Reporting System (TDRS).

OFA\'s state, territory, and tribal TANF grantees submit data to TDRS
that they are legislatively-mandated to report. OFA then aggregates the
data and uses it for descriptive analyses and program accountability,
most notably through the work participation rate calculations.

The existing system was developed in the late 1990s using late 80s
technology, possibly with some updates rolled in later on.

The states, territories, the District of Columbia, and
federally-recognized Indian tribes generally input their data in one of
several ways:

-   using a legacy tool (ftanf.exe) that exports files in a special text
    > format (information about the format of the incoming data can be
    > found here:
    > [[https://www.acf.hhs.gov/ofa/resource/tanfedit/index\#transmission-file-header]{.underline}](https://www.acf.hhs.gov/ofa/resource/tanfedit/index#transmission-file-header));

-   using their own software to export the data in this format; or

-   emailing their data to an OFA staff member to be input for them.

The data is then uploaded using SFTP into a system which then
periodically attempts to process the data and import it into the
database which the OFA staff uses for analysis. OFA staff accesses the
data via direct read-only SQL queries using tools like python, Jupyter
Notebooks, and SAS.

The database currently is around 50GB in size, though most of it is
historical data which will most likely not need to be migrated. Most of
the tables seem to contain between 700,000 to 1,300,000 rows and there
appears to be seven or so tables where most of the data is stored. These
tables are renamed periodically so there is a historical record. Access
to this data is extremely limited, both because the data is sensitive
(contains personally identifiable information or PII) and because
managing access to these aging systems is difficult.

## Problem

The current TDRS application was developed in the late 1990s and doesn't
take advantage of modern technology or best practices. The system is
inflexible to changing requirements, not automated, has no real user
interface, doesn't validate data effectively, and doesn't provide OFA
with full ownership of the data housed within it. This puts a
disproportionate amount of burden on all users of the system --- both
federal staff and the state, local, and tribal grantees --- and has led
to a painful user experience and often untimely or inaccurate data.

The data TDRS collects and stores from states, tribes, and territories
is critical to OFA's responsibility to report on the TANF program. The
data provides information about how states are meeting their participant
outreach targets, as well as demographic information about low-income
families.

High quality data leads to informed decision-making, and the TANF
program relies on this information to make policy recommendations.
Additionally, states and territories face penalties of up to four
percent of their total grant award each quarter if TDRS data is not
timely, complete, and accurate.

Issues with the current system prevent states from meeting their goals
and prevent the federal team from being able to accurately gauge TANF's
impact. Dealing with the deficiencies of the aging software is taking up
significant amounts of the OFA staff time.

## Vision

OFA will build a new, secure, web-based data system to improve the
federal reporting experience for states, tribes, territories, and
federal staff. A system that lets states, tribes, territories directly
upload and view the status of their data will reduce the burden on all
users, improve data quality, and ultimately help low-income families.
