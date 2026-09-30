# ADR-003: Use Django for the SEC Website Backend

**Date:** 2026-09-26  
**Author:** President  
**Owner:** President  
**Status:** Accepted

## Context

The SEC Website needs a backend foundation for website data, future protected features, and API development.

The initial proposed backend framework was Java with Spring Boot. During Sprint 1 planning, the club gained a Lead Engineer who actively uses Django and is available to mentor the Backend Pod. Because the club is new and members are learning the engineering workflow while building, active technical mentorship is a major delivery and learning factor.

## Decision Drivers

- Give the Backend Pod access to active, experienced mentorship
- Start Sprint 1 with a framework the Lead Engineer can review and support
- Keep the first project achievable for a new student organization
- Support a maintainable modular-monolith architecture
- Build a real backend while helping members learn the full engineering workflow

## Options Considered

### Option 1: Django

Use Django and Python for the SEC Website backend.

**Advantages**

- The Lead Engineer can mentor, review, and unblock the Backend Pod
- Django provides a mature foundation for web applications
- Python is accessible to members newer to backend development

**Tradeoffs**

- Existing Spring Boot references must be updated
- Members interested in Java and Spring Boot will not use it for this club project

### Option 2: Java with Spring Boot

Keep the original proposed Java and Spring Boot backend.

**Advantages**

- Strong alignment with common enterprise backend practices
- Supports members interested in Java backend development

**Tradeoffs**

- The club does not currently have the same level of hands-on Spring Boot mentorship
- Higher risk of slower early delivery and more unresolved questions during Sprint 1

## Decision

The SEC Website backend will use **Django**.

The website will remain a modular monolith. React remains the frontend framework, and PostgreSQL remains the selected relational database.

## Rationale

For the club's first active project, consistent mentorship and the ability to unblock contributors outweigh the benefit of keeping the originally proposed framework. Django lets the Lead Engineer provide practical guidance while members learn the full engineering workflow: issue, branch, pull request, review, test, and documentation.

This decision does not mean Django is universally better than Spring Boot. It is the better fit for the club's current mentorship capacity and Sprint 1 goals.

## Consequences

### Positive

- Backend contributors have a clear technical mentor
- The team can begin implementation with shared framework knowledge
- The club reduces early project risk while still building a production-oriented backend

### Negative

- Existing Spring Boot references must be changed to Django
- Java and Spring Boot learning remains an individual or future-project path rather than the current website backend
- Deployment research must evaluate platforms that support Python and Django

## Related Decisions and Work

- ADR-001: Use PostgreSQL as the relational database
- ADR-002: All club repositories are public
- Related issue: Set up Django backend and health endpoint
- Related architecture: SEC Website modular-monolith design
