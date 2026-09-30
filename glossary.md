# Engineering Glossary

**Purpose:** Define common SEC engineering terms in plain language.

**Intended audience:** New and returning SEC members.

**Last updated:** 2026-09-30  
**Owner:** President

## Core workflow terms

| Term | Meaning |
|---|---|
| Issue | A GitHub record describing one piece of planned work. |
| Acceptance criteria | A checklist that states what must be true for an issue to be complete. |
| Branch | A separate workspace for a change, created from `main`. |
| Commit | A saved checkpoint of related changes in Git history. |
| Pull request (PR) | A request to review and merge a branch into `main`. |
| Review | Feedback and approval from another contributor before a PR merges. |
| `main` | The protected, stable version of a repository. |
| GitHub Project | The board that shows issues, ownership, and work status. |
| Sprint | A short, focused period of planned work with a specific goal. |
| Pod | A small group organized around a work area, such as Frontend or Backend. |
| Blocker | Something preventing a task from moving forward. Report it in the relevant pod channel. |

## Architecture and documentation terms

| Term | Meaning |
|---|---|
| Modular monolith | One deployable application organized into clear internal modules, rather than many separate services. |
| API | A defined way for the frontend and backend to exchange information. |
| Endpoint | One API address that performs a specific action, such as `GET /api/health`. |
| ADR | Architecture Decision Record: a short document explaining a major technical decision and its reasoning. |
| CI | Continuous Integration: automated checks that run when code is pushed or a pull request is opened. |
| README | The starting document that explains a repository's purpose and setup. |

## Related documents

- [Engineering Principles](engineering-principles.md)
- [Git Workflow](engineering-standards/git-workflow.md)
- [First Contribution Guide](onboarding/first-contribution.md)
