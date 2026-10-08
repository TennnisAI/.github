<a href="https://getagency.dev">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/TennnisAI/.github/main/profile/assets/banner-dark.png">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/TennnisAI/.github/main/profile/assets/banner-light.png">
  <img src="https://raw.githubusercontent.com/TennnisAI/.github/main/profile/assets/banner-dark.png" alt="Many agents. Many branches. One window. Six agent lanes, Claude Code, Codex, Gemini CLI, OpenCode, Cursor and Copilot, fork off one trunk.">
</picture>
</a>

**Agency is a free, open-source desktop app that runs AI coding agents in parallel
on your own machine.** Claude Code, Codex, Gemini CLI and the other agent CLIs you
already use each get a real terminal, their own git worktree and their own branch.
You read the diffs and merge the good ones.

**[Download for macOS and Linux](https://getagency.dev/download)** &nbsp;&nbsp; [getagency.dev](https://getagency.dev) &nbsp;&nbsp; [Source](https://github.com/TennnisAI/Agency)

v0.2.3, in beta. macOS 11 or later on Apple Silicon, and Linux on x86_64 and
arm64. Free, Apache-2.0, and no account.

<a href="https://getagency.dev/#tour"><img src="https://raw.githubusercontent.com/TennnisAI/.github/main/profile/assets/hero.webp" alt="Agency running eleven agents across four projects, then six agents on one repo, four agents racing one prompt, and a branch merged cleanly into main."></a>

<sub>The app, running. [Watch the one-minute tour on getagency.dev.](https://getagency.dev/#tour)</sub>

## Works with what you already run

`Claude Code` `Codex` `Gemini CLI` `OpenCode` `Cursor` `Copilot CLI` `Kimi Code` `Crush` `Hermes` `Pi` `DeepSeek Harness` `any other CLI`

Bring the agents you already pay for. Agency finds what is on your PATH and
offers to install what is not. Your keys and subscriptions stay as they are.

## From an issue to a merged branch

Write the task down, give the agent the context, let several run at once, and
read every change before it lands on your base branch.

### 1. Plan: your tracker is a folder of markdown files

Issues live in your project as plain files. That is why an agent can work them:
picking one up, changing its status, commenting and filing a follow-up are all
just edits.

- Dispatch an issue to an agent and it moves to In progress
- Open a PR and it moves to In review. Merge and it closes
- Comments, links, attachments and due dates, all in the file

<img src="https://raw.githubusercontent.com/TennnisAI/.github/main/profile/assets/shot-issues.webp" alt="The Issues tab: a board grouped by Backlog, Todo, In progress and In review, with an issue open beside it showing its acceptance criteria, a comment and a linked issue.">

### 2. Context: notes your agents can actually read

A wiki that lives in your repo, with wikilinks, backlinks, tags, an outline and a
quick switcher, plus a journal with daily notes and a weekly note built from what
actually happened.

- Hand a note to an agent and watch the page update as it writes
- Put an agent in the side panel of the note you are working on
- Keep a notes-only workspace with no code in it at all

<img src="https://raw.githubusercontent.com/TennnisAI/.github/main/profile/assets/shot-docs.webp" alt="The Docs tab: an architecture note open with its properties, headings and a task list, the notes tree on the left, and the note's outline and backlinks on the right.">

### 3. Run: six agents, six branches, no collisions

Every run opens in its own git worktree: a second checkout of the same repo on
its own branch. Agents working the same project never touch each other's files.
Watch them all in a grid, or pull one full size when it needs you.

- Different agent CLIs on the same repo at the same time
- Plain terminals alongside, in the project checkout, when you want one
- Desktop alerts when an agent finishes, stalls on a question or hits a conflict

<img src="https://raw.githubusercontent.com/TennnisAI/.github/main/profile/assets/shot-grid.webp" alt="The Agents grid: six agents working one repo at once, Claude Code, Codex, Gemini CLI, OpenCode, Cursor and Pi, each tile showing its branch, its diff size and its live terminal.">

### 4. Review: read the diff before you trust it

Per-hunk diffs, commit, history, branches and stash for whichever worktree you
are standing in. Review a pull request, open one, merge it, and resolve the
conflicts when two agents reach for the same lines.

- Per-run diffs, so you review one agent's work at a time
- Comment on a diff and send it straight back to the agent

<img src="https://raw.githubusercontent.com/TennnisAI/.github/main/profile/assets/shot-merge.webp" alt="Source Control Changes: a side-by-side diff of an agent's fix to a flaky test, the commit form for its branch, and the branch history below.">

## The parts you notice on day two

|  |  |
|---|---|
| **&#x2273;&#xFE0E; Terminal first** | Agency does not reimplement your agent. It spawns the CLI you already use in a real terminal, TUI and all, and you can type into it. |
| **&#x21CB;&#xFE0E; Agent agnostic** | Eleven agent CLIs built in, and any other you can launch from a command line. Bring your own keys. |
| **&#x25A6;&#xFE0E; Many projects, one window** | Set agents going on one project, switch to the next, and come back when they are done. One home screen covers all of them. |
| **&#x25D4;&#xFE0E; Quiet until it matters** | Alerts when an agent finishes, goes quiet waiting on you, crashes a run script or hits a merge conflict. Silent for the run you are watching. |
| **&#x27F3;&#xFE0E; Auto-resume** | Quit with work in flight. Reopen, click the run, and the conversation picks up where the agent's CLI can continue it. |
| **&#x2225;&#xFE0E; Race and loop** | Send one prompt to four agents and keep the branch you like best. Or loop one agent until your test command exits clean, with hard caps on attempts, time and tokens. |

## No account. No vendor backend. No telemetry.

Agency does no first-party data collection, and there is no server of ours for it
to talk to. The coding agents are third party and talk to their own providers
with your own credentials, the same as when you run them in a terminal, and git
talks to whichever remotes you configured.

Agency makes one kind of network request of its own, the update check: on launch
and every six hours while it is open, it asks GitHub's public API for the latest
release tag and compares it to the version you are running. It sends no
identifiers and downloads nothing, and one switch in Settings turns it off. A
release is fetched only when you press Install, and it is checked against a
signing key built into the app before it goes in place.
[The privacy page](https://getagency.dev/privacy) has the full account.

## Agency built Agency

Almost everything above was written by agents running in Agency, on worktrees
Agency cut, then reviewed and merged in the app. The commit history is the
receipt, and it is public:
**237 agent branches merged into main, and 1,056 commits between 18 June and
6 October 2026.** [Read it.](https://github.com/TennnisAI/Agency/commits/main)

---

Pre-1.0 and in beta. Windows is planned. New to running agents side by side?
[Here is how to do it by hand](https://getagency.dev/run-coding-agents-in-parallel),
with or without Agency.

Brought to you by **[Tennnis](https://tennnis.no)**.
