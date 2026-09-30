# Git Workflow

**Purpose:** Define the required workflow for contributing to SEC repositories.

**Intended audience:** All SEC contributors and reviewers.

**Last updated:** 2026-09-30  
**Owner:** President

## Workflow

1. Find a GitHub issue in the Project board's **Ready** column.
2. Read the issue, including its acceptance criteria and dependencies.
3. Assign yourself as the issue owner before starting work.
4. Create a branch from `main`.
5. Make and test your changes locally.
6. Commit and push your branch.
7. Open a pull request into `main`.
8. Link the pull request to its issue and request review.
9. Address review feedback.
10. Merge only after the required approval and checks are complete.

## Branch names

Use one of these five prefixes:

| Work type | Branch format | Example |
|---|---|---|
| New feature | `feature/` | `feature/setup-django-backend` |
| Bug fix | `bugfix/` | `bugfix/fix-mobile-navigation` |
| Documentation | `docs/` | `docs/update-git-workflow` |
| CI or CD | `ci/` | `ci/add-backend-check` |
| Urgent production fix | `hotfix/` | `hotfix/restore-homepage` |

Use lowercase words separated by hyphens after the prefix.

## Commit messages

Use Conventional Commits:

```text
type: short description
```

Examples:

```text
feat: add health endpoint
docs: update git workflow
fix: correct mobile navigation spacing
```

## Pull request rules

- `main` is protected. Do not push directly to it.
- Every change must be submitted through a pull request.
- A pull request requires one approval and resolved review conversations before merging.
- Link the pull request to its GitHub issue.
- Do not merge your own pull request.
- Update documentation in the same pull request when behavior or setup changes.

## If you are blocked

Post in your pod's Discord channel:

1. What you were trying to do
2. What you tried
3. The error or unexpected result
4. A screenshot or pasted error message, when helpful

Asking for help early is part of the engineering workflow.

## Related documents

- [Engineering Principles](../engineering-principles.md)
- [Engineering Glossary](../glossary.md)
- [First Contribution Guide](../onboarding/first-contribution.md)
