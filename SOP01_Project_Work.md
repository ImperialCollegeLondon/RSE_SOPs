---
title: SOP-01 - Standard Operating Procedure for Software-Oriented Project Work
---

* TOC
{:toc}

##  1. Authorship 

-   Dr Diego Alonso Álvarez, RSE Team Lead


##  2. Version record

  | Version Number | Effective date | Reason for change   |
  | -------------- | -------------- | ------------------- |
  | 0              | 15 Sep 2021    | Creation of the SOP |
  | 0.1            | 3 Nov 2022     | Move to Markdown    |

##  3. Glossary

- **Software**: The target artefact of the project work. This might be a single piece of 
  software or several of them, it could be made of independent scripts, be a library or an 
  end-user executable, etc. It might already exist and need refactoring or be a new 
  creation that needs to be written from scratch.
- **Software components**: Each of the individual units the software is made from. They
  can be  fully independent or be related to each other in some form. Examples of
  components are graphical user interface, database, backend or business logic, API,
  etc.
- **Software description**: A description of a software's purpose, history, impact,
  existing  contributors- and user-bases. It is written as part of the planning process
  to ensure that the people involved know the context of the project, why the software
  is needed, what it will look like and who will benefit from it.
- **Scope**: Defines the boundaries of the project (what is and is not expected of the
  project)  and the software.
- **Stakeholder**: Anyone who has an interest in the project.
- **Task**: Something that needs to be done to complete the project. Can be split into
  sub-tasks. 
- **Project proposal**: Formal document that describes the overall project, the
  software, their  scopes, tasks to be performed and timeline for the completion of the
  project.

##  4. Introduction

Standard Operating Procedures (SOPs) are succinct formal documents designed to achieve
consistency in specified functions by defining a standard practice in performing those
functions.

This document forms part of the set of Standard Operating Procedures (SOPs) of Imperial
College RSE Team, part of the Research Computing Service (ICT) and describes the roles,
responsibilities, and actions necessary for the effective definition and management of
software-oriented project work.

##  5. Purpose

This SOP describes the principles of project work within the RSE Team that is mostly
software oriented. There is separate SOP (SOP-02) for those projects mostly about
training, mentoring and support researchers to create better software themselves. Some
projects might have a mix of both aspects. For those cases, relevant aspects of the two
SOPs will need to be considered.

This SOP covers the project initiation, planning, execution, monitoring, control,
closure, and potential follow ups. It also describes the actions and responsibilities
required to undertake these steps, as well as the tools, documents, and methods to be
employed.

To engage researchers effectively, the RSE Team needs to have some degree of flexibility
in the implementation of these procedures. Therefore, while this SOP defines the steps
that must be follow for each project in principle, there is scope for reasonable
adjustments should the specific project require them, and assuming they are properly
justified. Those situations will be evaluated on a case-by-case basis.

##  6. Roles and Responsibilities

-   **The Project Leader (PL)** is the member of the RSE Team (typically a Senior RSE)
    responsible for the overall delivery of the project and for the effective
    implementation of this SOP, with the support of the RSE Team Lead and the Lead
    Technologist.
-   **The RSE Team Lead** is responsible for approving the project proposal, prepare a
    quotation with timeline and costs -- already agreed in the project proposal --, and
    have it completed with a project code and a signature from someone able to approve
    the expenditure. It is also responsible for charging the costs of the project after
    the completion of agreed milestones. It supports the PL in the implementation of
    this SOP.
-   **The Technical Lead** is responsible for ensuring that the technology solutions
    defined in the project proposal are appropriate, achievable, and reusable in other
    projects, if relevant, advising the PL in that regard. It supports the PL
    interfacing with other teams and resources within ICT.
-   **The Project Team** is formed by all members of the RSE Team involved in the
    project and is responsible for effective application of the RSE Team Development
    Principles in pursuit of the objectives of the project. All members of the project
    team are required to follow the processes and procedures set out in this SOP.
-   **The Research Team** is formed by those researchers who are involved in the project
    and who are responsible for either actively contributing to the coding, providing
    domain knowledge, or testing the usability or performance of the features of the
    software. 
-   **The Research Leader (RL)** is (typically) the instigator of the project on the
    research side and is responsible for providing the PL with all the domain knowledge
    information and resources required for a successful and timely completion of the
    project. Might delegate some of these tasks to other members of the Research Team

##  7. Procedure

(Workflow summary)

###  7.1. Project initiation

A project starts with an Imperial researcher getting in touch with the RSE Team. This
first contact might follow different routes, including: 

-   Direct email to team members
-   Discussion in an HPC Clinic, Code Surgery or in the Imperial RS Community Slack
    workspace
-   Contacted via a ticket in ASK Imperial
-   FIXME: Fill of the [Software Information Gathering Questionnaire](https://forms.office.com/r/QAeQQZLhqv)
-   Face to face in conferences and other events

The members of the RSE Team might also actively seek new leads by contacting researchers
or groups of them (e.g. part of large consortia or Global Institutes) if the
opportunity arises.

A **senior member** of the RSE Team will be designated as the **Project Leader (PL)**
and will oversee setting up an initial meeting with the Research Leader to find out more
about the software and the overall scope for the project.

The specific actions for the PL at this stage are:

-   Setup an initial meeting with the Research Leader. The RSE Team Lead, the Lead
    Technologist and other members of the Research Team could be involved in this
    meeting, as required.
-   FIXME: Create a Wiki page for the project in the
    [RSE Team
    Wiki](https://wiki.imperial.ac.uk/display/IRSE/ICT+-+Research+Software+Engineering+Home),
    under Leads/{PL\_name}/{project\_or\_RL\_name}. Any notes from meetings, links to
    relevant resources, link to reports, etc. should be included here and kept up to
    date as the project evolves.
-   FIXME: Create a card
    in [Planner](https://tasks.office.com/ImperialLondon.onmicrosoft.com/Home/PlanViews/TJ05dTWhf0yrnsjaUdR4gJYABjFs?Type=PlanLink&Channel=Link&CreatedTime=637673125230370000)
    for the project, under the "Leads" bucket. Initially, this card will just contain
    the contact details of the RL -- and possibly other members of the Research Team --
    and a link to the Wiki page created above. 
-   If the [Software Information Gathering
    Questionnaire](https://forms.office.com/r/QAeQQZLhqv) has not been filled yet, it
    could be a good time to send it to the Research Leader to start the gathering
    information process.

###  7.2. Requirements and resources gathering

This step is all about the PL gathering all the relevant information about the software
-- and the project as a whole -- to decide if we can go ahead with the project. The
specific questions that need answering are:

-   Does it fit within one (or more) of the **RSE Team Strategic
    Objectives**?
-   Do we have the **technical expertise** for doing it?
-   Do we have the **capacity** (in principle) for doing it within the timeframe the
    researchers need?
-   Do we think we **will learn and enjoy** doing it?

A more exhaustive list of questions that could help with the project approval process
are included in [Appendix: Project selection criteria](#Projectselectioncriteria)

Therefore, this stage is a mixture of reviewing existing code, reading through web pages
and other resources, and talking to the researchers to find out any details we might
need to answer the questions above.

If the software already exists, this stage usually starts as a lightweight version of a
FIXME:[Code Audit](https://wiki.imperial.ac.uk/display/IRSE/Project+audit), followed by
a discussion with the RL and the Research Team to find out about the specific
requirements that the new software should fulfil.

All this information should be captured by the PL in the Wiki for the project.

Both the RSE Team Lead and the Technical Lead should be involved during or after the
information gathering process to help answering the above questions, considering their
broader understanding of the commitments of the RSE Team and the technical resources
available within ICT and Imperial.

If the answer is positive, in principle, the project moves to the next step, the
planning of the project proposal. Otherwise, the Project Leader will inform the Research
Leader of the reasons why the project cannot be accepted at this time, looking always
for a constructive way of supporting their needs -- pointing them to other resources
they might be able to use, to other teams or consultants who could potentially help
them, or suggesting ideas to reformulate the project so we can take it (or parts of it).
(FIXME: mention OSB and Code Surgeries.)

###  7.3. Planning of the project proposal

Planning and writing the project proposal is an iterative process to be written together
with the Research Leader any relevant member of the Research Team and the RSE Team Lead
and Technical Lead when appropriate. It aims to capture the specific scope of the
project, deliverables, features and timeline, as well as describing any aspects of the
project that might need clarification or agreed beforehand (like license issues,
reporting schedule, input data or resources from the Research Leader, etc.)

The **Project Template** contains all the relevant sections that need to be completed,
with hints on how to complete them, as well as some fixed sections containing
information of our Development Principles or about the Intellectual Property of the work
we do.

When starting this stage, the Project Leader will create a copy of the Project Template
in the SharePoint of the RSE Team under
[General/Projects/Leads](https://imperiallondon.sharepoint.com/:f:/r/sites/RSE/Shared%20Documents/General/Projects/Leads?csf=1&web=1&e=e17Ugf)
with the name of the project and share it with the Research Leader.

###  7.4. Project approval

###  7.5. Project start

###  7.6. Project delivery
    

####  7.6.1. Day-to-day project activity

####  7.6.2. Meetings

####  7.6.3. Reports

####  7.6.4. Contingency plans

###  7.7. Project closure


###  7.8. Follow up


##  8. References


##  9. Related SOPs and other documents

- RSE Team Principles -- aka "RSE Team World Domination Scheme"
- SOP-02: Standard Operating Procedure for Training Projects.
- Project proposal template
- Project report template
- Quotation template

##  10. Appendices

###  10.1. Project selection criteria

The following list compiles more concrete questions that could help to decide to go
ahead with a project, and that elaborate on the higher-level questions included in
Section 5.2. A project does not need to answer positively ALL of them to go ahead with
it, but we should try to give preference to those projects that tick more of them.

A more rigorous evaluation can be done using a [Criteria-Based Assessment for
software](https://software.ac.uk/sites/default/files/SSI-SoftwareEvaluationCriteria.pdf),
although such approach is a bit overkilling and probably not suitable for research
software, which often scores poorly in most metrics related to sustainability having
been developed organically by not expert coders over many years.

-   Expertise
    -   How quickly can we add value?
    -   Are we qualified to contribute to the project?
    -   Does the total of our technical knowledge, domain expertise and
        basic enthusiasm justify our involvement?
-   Skills development
    -   Does the project present an opportunity for us to acquire useful, transferable
        knowledge, either technical or domain-specific? 
-   Follow-on work
    -   Is the project likely to lead to further work with the same group or department?
    -   Has further funding already been secured?
-   Intrinsic value
    -   The [College](http://www.imperial.ac.uk/strategy/) have strategic plans that
        prioritise specific activities. Is the proposed project aligned with these? 
    -   Does the project genuinely accelerate, innovate, and strengthen research?
-   Does the PI:
    -   Understand our offering?
    -   Appreciate what we\'re able (and unable) to provide?
    -   Have realistic expectations of the collaboration?
    -   Understand the principles and challenges of software engineering?
-   Knowledge transfer
    -   Are there designated individuals within the research group who we will be
        working with? 
    -   Are they curious and enthusiastic about working with us?
    -   Will they be be given enough time to collaborate?
    -   Will they take their share of responsibility when it comes to
        delivering the project, and, most importantly, its long-term
        success?
-   Is the project possible?
    -   Is the codebase accessible?
    -   Is it (or could it be) tested?
    -   Is it clear who owns the code? Are they available?
    -   Is the research, whether it is pre- or post-publication, documented?
    -   Are there clear acceptance criteria and/or deliverables?
    -   Is any existing code intelligible?
-   HPC
    -   Is there potential to make use of (and sell) other services provided by the RCS and/or ICT? Training, HPC, infrastructure\...
