# ADR-001: Use PostgreSQL as the Relational Database

**Date:** 2026-08-09  
**Author:** President  
**Owner:** President  
**Status:** Accepted

## Context

The SEC Website needs a relational database for approved website information and future backend features.

The database choice should support the website's modular-monolith architecture, work well with Django, and remain a practical option for a student organization as the project grows.

## Decision Drivers

- Support reliable relational data and clear relationships between records
- Work well with Django and future deployment platforms
- Use a widely adopted, production-capable database
- Give members experience with a common backend technology
- Keep the database choice maintainable as the project grows

## Options Considered

### Option 1: PostgreSQL

Use PostgreSQL as the SEC Website's relational database.

**Advantages**

- Mature, open-source, production-capable relational database
- Strong support in Django and common hosting platforms
- Supports clear data relationships, constraints, and structured queries
- Relevant experience for backend contributors

**Tradeoffs**

- Requires database setup beyond a simple local file
- Adds configuration and deployment work compared with a temporary local-only database

### Option 2: SQLite

Use SQLite as the primary database.

**Advantages**

- Simple local setup
- Included with many development environments

**Tradeoffs**

- Less suitable as the primary shared production database
- Does not provide the same operational experience as PostgreSQL
- May require a later migration as the project grows

## Decision

The SEC Website will use **PostgreSQL** as its relational database.

## Rationale

PostgreSQL provides a stable, production-capable relational database that works well with Django and gives the Backend Pod experience with a commonly used database technology. It is a stronger long-term fit than a local-only database while remaining accessible for a student project.

## Consequences

### Positive

- The project has a clear relational-database standard
- Django backend work can use a well-supported production database
- Contributors gain practical PostgreSQL experience

### Negative

- Local setup and deployment require database configuration
- The team must document connection settings and keep credentials out of the repository

## Related Decisions and Work

- ADR-003: Use Django for the SEC Website Backend
- Related architecture: SEC Website modular-monolith design
- Related work: SEC Website database setup task
