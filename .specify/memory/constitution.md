# Lab-Spec-Kit-training-10-29-2026 Constitution

## Core Principles

### I. Requirements Before Implementation
For planned feature work, contributors MUST document the user need, observable
outcomes, and relevant constraints in a specification before implementation.
Plans and tasks MUST remain traceable to those requirements. This keeps changes
focused on the intended outcome rather than assumptions.

### II. Prefer the Simplest Compatible Design
Contributors MUST prefer the smallest design that satisfies the stated
requirements and fits the existing project. New dependencies, abstractions, and
configuration MUST have a documented need. Existing behavior and interfaces
MUST be preserved unless a change is explicitly required.

### III. Verify Changes at the Right Scope
Changes MUST be validated with the narrowest applicable checks, such as focused
tests, builds, or static checks. Bug fixes MUST include verification of the
reported behavior when practical. If a relevant check cannot be run, the
limitation MUST be stated in the change description.

### IV. Keep Changes Reviewable
Each change MUST be scoped to a coherent user or maintenance outcome.
Documentation and tests MUST be updated when behavior or usage changes.
Contributors MUST avoid unrelated edits so reviewers can assess impact clearly.

### V. Make Decisions and Limitations Explicit
Specifications, plans, and code reviews MUST distinguish confirmed requirements
from assumptions. Non-obvious tradeoffs, compatibility impacts, and known
limitations MUST be recorded where maintainers can act on them.

## Project Constraints

The application MUST be built entirely on Microsoft Power Apps as a model-driven
app using Microsoft Dataverse. Features and data MUST use this platform;
contributors MUST NOT introduce a separate application platform or data store
without an approved constitutional amendment. This constraint keeps the product
within the platform explicitly selected for it.

The product is the Unauthorized Deductions Log (UD/UA), named
"Bitácora de Deducciones No Autorizadas (UD/UA)". Its scope MUST be limited to
recording unauthorized deductions and tracking them until UD closes or corrects
them. The earlier hardware-request scenario is not part of this product scope.

The application MUST NOT include connections to SAP, TNET, or TradePro,
notifications, or reports within the current scope. Recording an SAP document
number or an F-28/F-30 transaction reference MUST NOT imply executing a
transaction in SAP. These boundaries keep the app a tracking tool rather than
an integrated transaction-processing system. Expanding these boundaries MUST
follow the constitutional amendment procedure.

## Development Workflow

Feature work MUST use the repository's Spec Kit workflow to specify, plan, and
break down implementation before coding. Contributors SHOULD clarify material
ambiguities and analyze generated artifacts before implementation. Completed
changes MUST be reviewed and verified against their specification or stated
maintenance goal before integration.

## Governance

This constitution governs project work alongside applicable repository
configuration and security requirements. Amendments MUST be made through a
reviewable change that explains the reason and impact, and MUST be approved
through the repository's normal review process.

The constitution version follows semantic versioning: MAJOR for incompatible
changes to existing principles or governance, MINOR for new principles or
material expansions, and PATCH for clarifications and non-semantic edits.
Implementation plans and reviews MUST consider these principles; reviewers
MUST call out material noncompliance, and exceptions MUST document their
rationale and scope.

**Version**: 2.1.0 | **Ratified**: 2026-10-29 | **Last Amended**: 2026-10-29
