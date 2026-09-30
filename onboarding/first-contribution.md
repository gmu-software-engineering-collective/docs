# First Contribution Guide

**Purpose:** Walk a member through their first SEC contribution from issue selection to pull-request review.

**Intended audience:** SEC members making their first repository contribution.

**Last updated:** 2026-09-30  
**Owner:** President

## Before starting

Make sure you:

- Have access to the SEC GitHub organization
- Have completed the project-specific local setup from that repository's README
- Have read the [Git Workflow](../engineering-standards/git-workflow.md)
- Can identify your pod's Discord channel

## 1. Choose a ready task

1. Open the GitHub Project board.
2. Look in the **Ready** column.
3. Open an issue and read its problem, goal, acceptance criteria, dependencies, and research requirements.
4. Assign yourself only if you can own the task.

One issue has one owner. Other members may pair, research, test, or review.

## 2. Create your branch

Start from the current `main` branch:

```bash
git checkout main
git pull origin main
git checkout -b feature/short-task-name
```

Example:

```bash
git checkout -b feature/setup-django-backend
```

## 3. Make and test your change

Work only on the issue you selected. Use the issue's acceptance criteria as your checklist.

Run the project and any relevant tests before committing.

If you become blocked, post in your pod channel:

- What you were trying to do
- What you tried
- The error or result
- A screenshot or pasted error, if helpful

## 4. Commit and push

Use a Conventional Commit message:

```bash
git add .
git commit -m "feat: short description of change"
git push -u origin feature/short-task-name
```

Example:

```bash
git commit -m "feat: add Django health endpoint"
```

## 5. Open a pull request

1. Open the repository on GitHub.
2. Create a pull request from your branch into `main`.
3. Complete the pull-request template.
4. Link the pull request to its GitHub issue.
5. Request a review.

Do not merge your own pull request. Address review feedback, then wait for the required approval before merging.

## After merge

Confirm that the linked issue is closed and its Project board card is moved to **Done**.

## Related documents

- [Welcome Guide](welcome-guide.md)
- [Local Setup](local-setup.md)
- [Git Workflow](../engineering-standards/git-workflow.md)
- [Engineering Glossary](../glossary.md)
