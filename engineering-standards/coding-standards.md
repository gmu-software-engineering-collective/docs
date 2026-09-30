# Coding Standards

**Purpose:** Define the shared code-quality expectations for SEC repositories.

**Intended audience:** All SEC contributors and reviewers.

**Last updated:** 2026-09-30  
**Owner:** President

## Core standards

- Follow the existing structure and conventions of the repository you are changing.
- Prefer clear names over clever abbreviations.
- Keep each change focused on its linked GitHub issue.
- Do not add unused code, dependencies, files, or commented-out code.
- Keep functions and components focused on one clear responsibility.
- Avoid duplicating logic when an existing shared solution fits.
- Add or update tests when behavior changes.
- Update documentation when setup, behavior, or a public interface changes.
- Never commit secrets, credentials, or environment files.

## Formatting and linting

Each repository may define its own formatter, linter, and test commands in its README or configuration files.

Run the repository's documented checks before opening a pull request. Do not introduce a new formatting tool or major code pattern without discussing it in the relevant pod.

## Review expectations

Reviewers check whether a change:

- Meets the linked issue's acceptance criteria
- Matches the agreed architecture and repository structure
- Is understandable to another contributor
- Includes appropriate tests and documentation
- Introduces no obvious security or maintainability problems

## Related documents

- [Engineering Principles](../engineering-principles.md)
- [Git Workflow](git-workflow.md)
- [Security Checklist](security-checklist.md)
