# Security Checklist

**Purpose:** Give every SEC contributor a short security check before code is submitted for review.

**Intended audience:** All SEC contributors and reviewers.

**Last updated:** 2026-09-30  
**Owner:** President

## Before opening a pull request

- [ ] No passwords, API keys, tokens, private keys, or credentials are committed.
- [ ] Sensitive configuration is stored in environment variables, not source files.
- [ ] `.env` files and other local secrets are ignored by Git.
- [ ] User input is validated where it enters the application.
- [ ] Error messages do not expose stack traces, credentials, database queries, or internal details.
- [ ] Sensitive information is not written to logs.
- [ ] New dependencies are necessary and come from a trusted source.
- [ ] Documentation is updated if setup, behavior, or security expectations changed.

## When authentication is added

- [ ] Authentication and authorization are handled separately.
- [ ] Protected routes require authentication.
- [ ] Users can access only the data and actions they are authorized to access.
- [ ] Passwords are never stored or logged in plain text.

## If you find a security issue

Do not post sensitive details in a public GitHub issue or Discord channel.

Follow the repository's Security Policy or contact a club officer privately with:

- A short description of the issue
- The affected repository or feature
- Steps to reproduce, without exposing credentials or private data
- The potential impact

## Related documents

- [Engineering Principles](../engineering-principles.md)
- [Git Workflow](git-workflow.md)
- [SEC Website Security Policy](https://github.com/gmu-software-engineering-collective/website/security/policy)
