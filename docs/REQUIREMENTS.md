# Letsflow requirements document
version 1.0.0

# Methods

* represent all features as Gherkin feature files


# Questions 

* what attributes should templates have and what form should they take?

* how should the system represent companies that have multiple divisions or locations or departments?

* how should be organize templates so they are easy to find an use?

* how should reporting and dashboards work given the answers to the previous questions?

* how should integrations ( Zapier etc ) work in future and what design decisions need to be made now?

# MVP requirements

* a company regardless or its structure will have policies and procedures modeled by business processes

* the ability to model a business process aids in training new and existing employees

* the ability to reproduce reports and actions taken for a process aids in compliance and auditing

* reusable templates can represent a business process

* templates will need to be identified

* it is easier to update software in a single system than across multiple systems

* initially companies will use a shared system, that is multiple companies will be in a single database

* template can be modified to improve process after initial usage, therefore versioning will be required

* given the previous requirements, templates must have a primary key id, version, company id

* templates will need attributes and multiple categorization support for reporting purposes

* structural design of system should plan for attributes on templates that can be carried onto generated tasks

* some business processes have dependencies, while others can happen concurrently

* system should support parallel tasks that work like a simple checklist that can be done out of order

* system should support serial tasks that require one task to be completed before the other

* serial tasks imply a parent child relationship

* serial and parallel tasks can be combined in a single process

* tasks with more than one parent are implied by the nature of mixing serial and parallel tasks 

* tasks can have attachments notes, and comments 

* tasks can be incomplete or complete, this implies a state attribute of the task

* PII and GPDR European privacy data can possibly be added in attachments, notes, and comments, so we need to secure information

* https must be used for all interaction with the system

* possibility for encryption of notes and attachments must be planned for in design due to new privacy laws

* a completed set of tasks generated from a template is archived and available for reproduction for audit purposes

* sets of tasks described by a template can be created by manual, triggered, or scheduled.

* tasks can be configured such that only certain entities with certain roles can complete the task

* a simple role based system should be considered for access control admin and user initially

* only a template creator or admin can change an existing template

* simple dashboard and simple UI 

* simple preset report system

* avoid more than one way to do something, make pragmatic choices that work for 80% of cases 80/20



# Phase 2 requirements after MVP

* tags offer more flexibility than single categories, therefore we should use tags for attributes and categories

* tags themselves should have a type

* custom tags will be needed as different companies have different needs, therefore tags and type should be both be generally available as well as identified by a single company

* sets of tasks generated from a template might need to inherit tags from the template

* access control on tasks may also imply access control on templates ???

* integrations

* free training videos to ensure all users are trained

