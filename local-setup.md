# Local Setup

**Purpose:** Explain the minimum setup needed before contributing to an SEC project.

**Intended audience:** SEC members preparing to make their first contribution.

**Last updated:** 2026-09-30  
**Owner:** President

## Before you start

You need:

- A GitHub account
- Access to the SEC GitHub organization
- Git installed on your computer (https://git-scm.com/)
- A code editor or IDE
- The tools listed in the specific project's README

For the SEC Website, the project README is the source of truth for the required Python, Django, Node.js, React, database, and run-command setup.

## First-time Git configuration

Set your Git name and email once on your computer:

```bash
git config --global user.name "Your Name"
git config --global user.email "your-github-email@example.com"
```

Use the same email connected to your GitHub account.

## Clone a repository

After you have organization access, clone the repository you are contributing to:

```bash
git clone https://github.com/gmu-software-engineering-collective/website.git
cd website
```

Then follow that repository's README to install its dependencies and run the project locally.

## Important rule

Do not guess project versions, commands, or folder structure. Read the repository README first, then ask your pod channel if something is missing or unclear.

## Related documents

- [Welcome Guide](welcome-guide.md)
- [First Contribution Guide](first-contribution.md)
- [Git Workflow](../engineering-standards/git-workflow.md)
