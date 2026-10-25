# Personal AI System

A personal AI assistant with a memory you control.

This public repository is a reusable template. It gives Codex, Claude, ChatGPT
or another compatible assistant a durable source of truth made from plain
Markdown files. You talk to the assistant; it reads and updates your personal
working copy when something is worth remembering. Your memory stays visible,
portable and under your control.

## Quick start prompt

Copy this message into an AI assistant that can help you work with files or
GitHub:

```text
Help me set up my Personal AI System using the public template at
https://github.com/pabloalbian/personal-ai-system.

This may be a copied prompt, so do not infer my preferred language from its
wording. Start by asking which language I want to use, then continue in it.

First, determine what you can actually access: writable local files and Git, a
cloud workspace connected to GitHub, GitHub with read or write access, or none
of these. Do not assume that I already have Git or a GitHub account. Briefly
explain the most suitable option for my situation and guide me one step at a
time.

The public repository is the template, not the place for my personal data. The
goal is to create or reuse my own working copy and keep any remote copy private
by default. Never write my personal information to the public template.

If I already have a personal copy, reuse it without overwriting existing files.
If I am working through GitHub or a cloud environment and do not have one, help
me create a new private repository from the template. If you can perform that
action, ask for my approval first; otherwise guide me through it one step at a
time. Then work only inside my private copy.

If I am working locally without a GitHub copy, clone or download the public
template into a suitable new folder. If Git is unavailable, help me choose
between installing it and downloading the template, but do not install software
without asking.

A GitHub account is not required for local use. Explain when an account would
be useful for a private remote copy, syncing, Codex Cloud or another GitHub-based
assistant connection.

Do not overwrite existing files, create an account, publish personal content,
change repository visibility, commit or push unless I explicitly approve the
relevant action.

Once the repository is available, work inside it and read `README.md`,
`AGENTS.md` and `Preferences.md`. Then begin its guided onboarding in the
language I am using. Ask one question at a time; I should not need to understand
the file structure before we begin.
```

You may translate or adapt the message. The setup should continue in the
language you use.

A GitHub account is not required to clone or download the template for local
use. It becomes relevant if you want a private remote copy, syncing, Codex Cloud
or another GitHub-based assistant connection.

## Choose where to use it

- **Local:** clone or download the template and let a compatible assistant work
  with the files on your computer. A GitHub account is optional.
- **In a cloud coding environment:** create a private repository from the
  template, connect that copy to the environment and let the assistant work
  there. This is the most direct route when you want to use the system entirely
  from the web.
- **In a regular chat:** the assistant can guide the setup, but it can maintain
  the system only if that chat has write access to your personal repository. If
  it has read-only access or no persistent storage, use a local or cloud coding
  environment for the actual setup.

## Saving and syncing

When the assistant saves a task, preference or note, it first changes the files
in the working copy used by the current session. Those changes will not
automatically appear in another checkout or in a new session that reads the
remote repository.

After a meaningful group of changes, the assistant will tell you where the work
is saved and ask whether you also want to synchronise it with your private remote
copy. If you prefer technical detail, it will call this making a commit and
pushing it. It should ask at a natural stopping point rather than after every
small edit, and it will not commit or push unless you approve that specific
action.

If you do not have a remote repository, local use still works normally. The
assistant can explain how to create a private remote copy if you want syncing or
access from other devices.

## Keep your personal copy private

This public repository is a reusable starting point. Once you begin adding your
own tasks, projects, preferences, messages or schedule, treat your working copy
as private. If you create a remote repository for syncing or backup, make it
private unless you deliberately choose to publish its contents.

Never store passwords, access tokens, cookies or integration credentials in the
repository. Connections to external services should be authorised and managed
by the AI tool or operating environment you are using.

## Start here

If you already have the repository open with an AI coding assistant, you can use
the shorter opening message:

> Help me set up my Personal AI System.

The assistant will briefly explain how the system can help and invite you to
start with one real thing you currently have pending. It can be a small task,
something you have been postponing or a larger outcome with several steps. You
can describe it naturally; the assistant will decide how to organise it and ask
only when an important detail needs clarification.

The assistant should guide the rest. You do not need to design a folder
structure, learn the repository model or arrive with a perfectly formed request.

## A guided first conversation

The first conversation is a short discovery process, not an empty chat prompt
and not a life-audit questionnaire. The assistant will:

1. introduce itself as a general assistant for organising and following up on
   the things you have to do;
2. explain that it can handle a small task, a multi-step outcome, a daily plan
   or context worth keeping over time;
3. invite you to bring one real thing you currently have pending;
4. use that example to find a useful next step and decide internally how it
   should be organised;
5. agree on the language for stored information and how much technical detail
   you want to see;
6. explain the difference between saving changes locally and synchronising them
   so they are available elsewhere; and
7. optionally mention calendar, email and messaging integrations, which you can
   configure now or leave for later.

You do not need to choose between tasks, projects or areas before you begin.
When that distinction matters, the assistant will ask in ordinary language.
You can skip questions or change the setup later, and mentioning a topic does
not automatically create a folder or permanently add it to the system.

## Use any language

Talk to the assistant in the language that feels natural to you. You can also
switch languages during a conversation. By default, the assistant replies in
the language of your current message.

During onboarding, the system chooses a primary language for the information it
stores so that individual files remain easy to read and do not become an
accidental mixture of languages. This preference can be changed later. Changing
the conversation language does not automatically translate or rewrite existing
files.

The template keeps stable names such as `Todo.md`, `Projects/`, `Areas/` and
`Daily/` for portability across tools and documentation. You do not need to use
or remember those names when talking to the assistant.

## How it grows

The initial system is intentionally small:

- `Todo.md` contains open actions.
- `Preferences.md` contains useful interaction preferences.
- `AGENTS.md` tells the assistant how to maintain the system safely.
- `CLAUDE.md` makes the same instructions available automatically to Claude
  Code.

When the need appears, the assistant can propose adding:

- `Projects/` for finite outcomes with several steps;
- `Areas/` for ongoing responsibilities; and
- `Daily/` for an agreed plan tied to a date.

These are not requirements. The structure should grow from real use instead of
starting as a collection of empty templates.

## Where tasks live

The system starts with one central list: every open action goes into `Todo.md`,
including actions connected to a project. When useful, a task links to its
project for context.

The assistant does not ask you to configure this during onboarding. When a
project first becomes substantial enough that keeping its actions alongside its
context could help, the assistant offers a choice:

- keep every open action in the central list; or
- keep standalone actions in `Todo.md` and project actions in their project.

This preference applies to future projects, so the assistant should not ask the
same question repeatedly. Either way, asking for all your open tasks includes
actions from every project. A task is stored in one place only; general and
filtered views are generated without copying it.

When you confirm that a task is complete, the assistant removes it from the
open list. It preserves the result only when it will be useful later—for
example, as a project milestone, decision or meaningful change of state. The
system does not build a permanent archive of routine completed tasks by default;
committed changes can still be recovered through Git history when necessary.

## What gets remembered

The guiding rule is:

> Start with the conversation. Persist only what will be useful later.

Exploring an idea does not automatically create a task or a file. Explicit
requests such as "remember this", "add this to my tasks" or "create a project"
do. The assistant should update an existing source of truth whenever possible
and keep durable notes concise.

## Example

Suppose a fictional user says:

> I may learn Italian one day. For now, add a task to compare two beginner
> courses by Friday.

The possibility of learning Italian can remain in the conversation. The course
comparison is a concrete task and belongs in `Todo.md`. The assistant should not
create an `Areas/Language Learning/` hierarchy or invent a deadline date without
enough information.

## Principles

- Conversation first, files when useful.
- One canonical source for each piece of information.
- Minimal structure that can evolve.
- No invented facts, deadlines or completed work.
- No publication, commits or pushes without an explicit request.
- Plain files that remain usable across tools and models.
