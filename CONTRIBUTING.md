# Contributing to erm-git repositories

These rules apply to every erm-git repository that does not have its own `CONTRIBUTING.md`
(GitHub serves this file as the default; see
[Creating a default community health file](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)).
They are for people and for AI agents alike. Each repository's `AGENTS.md` adds what is
specific to that repository.

Each rule below follows GitHub's documentation; the source is linked. Where GitHub leaves a
choice open, the line says **(choice)**.

## Issues

- Use an issue for anything that needs to be tracked or discussed: ideas, tasks, bugs, findings.
  ([About issues](https://docs.github.com/en/issues/tracking-your-work-with-issues/learning-about-issues/about-issues))
- One issue per problem or finding. Open it when it is found, even before it is confirmed.
- Use the issue forms offered when you click **New issue**.
  ([Issue templates](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/configuring-issue-templates-for-your-repository))
- Comments add evidence, results or decisions, not progress chatter.
- Never edit an issue's original title or body; add corrections and updates as comments so every change
  stays visible in the timeline **(choice)**.
- Close with a reason ([state reasons](https://docs.github.com/en/rest/issues/issues#update-an-issue)):
  - **Completed**: resolved.
  - **Not planned**: will not be done, or the finding turned out to be wrong.
  - **Duplicate**: already tracked elsewhere; link the other issue.

## Labels

Use GitHub's default labels
([Managing labels](https://docs.github.com/en/issues/using-labels-and-milestones-to-track-work/managing-labels)):

| Label | Use |
| --- | --- |
| `question` | Needs more information. Every finding that is not yet confirmed carries it; remove it once the evidence confirms the finding. |
| `bug` | Something does not work as intended. |
| `enhancement` | New capability. |
| `documentation` | Documentation needs adding or fixing. |
| `invalid` | No longer relevant, or disproved (close as Not planned). |
| `duplicate` | Same as another issue (close as Duplicate). |
| `wontfix` | Will not be worked on. |
| `help wanted`, `good first issue`, `accessibility` | As GitHub defines them. |

Extra label: `security` for security-relevant issues **(choice)**.

## Grouping and progress

- **Sub-issues** break a larger piece of work into tasks (up to 100 per parent, 8 levels, across
  repositories). Do not use them just to group related issues.
  ([Sub-issues](https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/adding-sub-issues))
- **Milestones** (or labels) tie items to a larger goal or phase.
- **Projects** hold the cross-repository view; extra metadata goes into project fields.
  ([Best practices for Projects](https://docs.github.com/en/issues/planning-and-tracking-with-projects/learning-about-projects/best-practices-for-projects))
- Keep one source of truth: the issue. Do not copy its content into other documents.

## Pull requests

- Work on a branch, never directly on the default branch. Branch name `<author>/<topic>-<yyyymmdd>` **(choice)**.
- Every change gets a pull request; the repository owner reviews and merges.
- Link the issue it resolves with a closing keyword in the description: `Closes #12`, `Fixes #12`,
  `Resolves #12` (other repository: `Closes owner/repo#12`). Keywords only work when the pull
  request targets the default branch.
  ([Linking a pull request to an issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/linking-a-pull-request-to-an-issue))
- Use the pull request template.

## AI agents

- Read the repository's `AGENTS.md` first; it says what is specific to that repository.
- **Read-only** means no edits or changes to any system (configs, services, files, data, settings,
  repository content). It does include: commands that only query, writing reports and the scratch or
  tool files needed to produce them, and opening, commenting on, labelling and closing issues **(choice)**.
- Read-only work is always fine. Any change needs the owner's approval and goes through a branch and a
  pull request.
- When a check needs access the agent does not have (root, a login, an API key), say so with the exact
  command or step for the owner, and keep it listed until it is done **(choice)**.
- Say which agent and model did the work in the issue or pull request.
