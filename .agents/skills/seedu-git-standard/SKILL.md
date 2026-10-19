---
name: seedu-git-standard
description: Apply this project's SE-EDU Git conventions when preparing, reviewing, or amending commit messages and when naming branches.
---

# SE-EDU Git standard

Source: [SE-EDU Git conventions](https://se-education.org/guides/conventions/git.html).

## Commit messages

- Aim for a subject of at most 50 characters; never exceed 72.
- Use an imperative subject, capitalize its initial letter, and omit the final period.
- An applicable scope or category prefix is optional; it does not require adopting Conventional Commits.
- Include a body for non-trivial changes. Leave an empty line after the subject, wrap body lines at 72 characters, and separate paragraphs with empty lines. Use bullets when helpful.
- Explain the change and its motivation, leaving implementation mechanics to the diff. Provide enough context to assess the change without reading code; avoid duplicating code comments.
- Organize the body around the existing situation (present tense), the need for change, the action (imperative), the rationale for the approach, and other relevant information.
- Omit redundant time qualifiers when describing the existing situation. An overlong explanation suggests splitting the commit.

## Branch names

Use descriptive kebab-case keywords. For issue work, use `<issue-number>-<issue-keywords>`.

## Project workflow

Before committing, inspect the staged diff, ensure the message accurately describes it, and check the rules above. Keep unrelated user changes out of the commit. Reading this skill does not authorize a commit or a history rewrite.

If the environment requires a branch namespace such as `codex/`, apply the naming rules to the portion after that prefix.
