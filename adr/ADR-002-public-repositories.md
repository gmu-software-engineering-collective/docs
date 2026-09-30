# ADR-002: All Club Repositories Are Public

**Date:** 2026-08-09  
**Author:** President  
**Owner:** President  
**Status:** Accepted

## Context

The club produces work that members may want to show in resumes, portfolios, and applications. It also produces documentation intended to outlive its original authors.

GitHub can host private repositories on the free plan, so public visibility is a deliberate choice rather than a limitation.

## Decision Drivers

- Let members share their work without requesting access
- Let prospective members see how the club operates
- Create documentation that remains accessible to future leadership
- Encourage a higher standard for code, documentation, and review
- Keep repository visibility consistent across the organization

## Options Considered

### Option 1: Public repositories by default

Make every club repository public unless a specific exception is approved.

**Advantages**

- Members can link their work publicly
- Club processes and documentation are transparent
- Future members can learn from existing work
- Public visibility creates a consistent quality standard

**Tradeoffs**

- Work in progress, including mistakes, is visible
- Contributors must be careful never to commit sensitive information

### Option 2: Private repositories by default

Make repositories private unless a repository is explicitly published.

**Advantages**

- Work in progress is visible only to organization members
- Less public exposure while contributors are learning

**Tradeoffs**

- Members cannot easily show their work
- Future members and prospective members cannot easily learn from club history
- Documentation requires access management

## Decision

Every repository in the Software Engineering Collective organization is **public by default**.

Making a repository private requires a separate ADR.

## Rationale

Members can link public repositories in resumes or applications without requesting access. Prospective members can see how the club actually works before joining. Public work also raises the standard of what is merged because the audience is not only the current club members.

Repository visibility changes are disabled at the organization level so this decision is enforced by tooling rather than trust alone.

## Consequences

### Positive

- Members can publicly demonstrate their contributions
- Club standards and documentation remain accessible
- The organization builds a transparent record for future leadership

### Negative

- No secrets, credentials, tokens, or private information may be committed
- Contributors must use environment variables and GitHub Actions secrets for sensitive configuration
- Work in progress is visible, including mistakes

## Related Decisions and Work

- [Engineering Principles](../engineering-principles.md)
- [Security Checklist](../engineering-standards/security-checklist.md)
- ADR-001: Use PostgreSQL as the Relational Database
- ADR-003: Use Django for the SEC Website Backend
