# Contributing

Thank you for contributing to the Software Engineering Collective.

All contributions follow the club's engineering workflow and published engineering standards.

## Before You Start

Every change begins with a GitHub Issue.

Before starting implementation:

- Make sure the issue clearly describes the problem and goal.
- Make sure acceptance criteria are defined.
- Confirm any dependencies.
- Complete required research.
- Assign the issue to yourself.

## Branches

Create your branch from the appropriate base branch.

Use one of the following branch prefixes:

- `feature/` for new features
- `bugfix/` for bug fixes
- `hotfix/` for critical production fixes
- `docs/` for documentation changes
- `ci/` for CI/CD changes

Use lowercase words separated by hyphens.

Examples:

`feature/auth-login`

`bugfix/footer-spacing`

`docs/onboarding-guide`

**Copy and paste:**

Create a new branch using the appropriate prefix.

```bash
git switch -c feature/auth-login
```

Other examples:

```bash
git switch -c bugfix/footer-spacing
git switch -c hotfix/session-crash
git switch -c docs/onboarding-guide
git switch -c ci/github-actions
```

Replace the branch name with a short description of your work.

## Commits

Use Conventional Commits.

Examples:

`feat(auth): add session middleware`

`fix(login): handle missing email`

`docs(readme): update local setup`

`test(auth): add registration tests`

`ci(actions): cache dependencies`

**Copy and paste:**

Use the appropriate commit type to describe your changes.

```bash
git commit -m "feat(auth): add session middleware"
```

Other examples:

```bash
git commit -m "fix(login): handle missing email"
git commit -m "docs(readme): update local setup"
git commit -m "test(auth): add registration tests"
git commit -m "ci(actions): cache dependencies"
```

Replace the commit type, scope, and description to match your changes.

## Pull Requests

All changes must be submitted through a pull request.

Before requesting review:

- Link the related issue.
- Explain what changed and why.
- Explain how the change was tested.
- Complete the pull request checklist.
- Make sure all acceptance criteria are satisfied.

At least one approving review is required before merge.

Do not push directly to protected branches.

## Engineering Standards

Detailed engineering standards are maintained in the organization's `docs` repository.

Follow the published Git workflow, coding standards, security requirements, and other applicable engineering documentation.
