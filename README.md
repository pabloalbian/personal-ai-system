# Personal AI System

A personal AI assistant with a memory you control.

This repository gives Codex, Claude, ChatGPT or another compatible assistant a
durable source of truth made from plain Markdown files. You talk to the
assistant; it reads and updates the files when something is worth remembering.
Your memory stays visible, portable and under your control.

## Quick start prompt

Copy this message into an AI assistant that can help you work with files or
GitHub:

```text
Help me set up my Personal AI System from
https://github.com/pabloalbian/personal-ai-system.

First, determine what you can actually access: local files and Git, a connected
GitHub account, or neither. Do not assume that I already have Git or a GitHub
account. Briefly explain the most suitable option for my situation and guide me
one step at a time.

This may be a copied prompt, so do not infer my preferred language from its
wording. Start by asking which language I want to use, then continue in it.

If you can work locally, clone the public repository into a suitable new folder,
or reuse an existing copy without overwriting it. If Git is unavailable, help me
choose between installing it and downloading the repository, but do not install
software without asking. If you can only work through GitHub, explain the access
or account step I need instead of pretending you can use my computer.

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

A GitHub account is not required to clone or download a public repository for
local use. It becomes relevant if you want a remote personal copy, syncing or a
GitHub-based assistant connection. The setup assistant should explain that
choice when it applies.

## Start here

If you already have the repository open with an AI coding assistant, you can use
the shorter opening message:

> Help me set up my Personal AI System.

The assistant will explain the system and ask which parts of your life you want
help with. You can answer with one current concern, several areas or simply say
that you are not sure. Together, you will choose a small starting point, the
language for stored information and how much technical detail you want to see.

The assistant should guide the rest. You do not need to design a folder
structure, learn the repository model or arrive with a perfectly formed request.

## A guided first conversation

The first conversation is a short discovery process, not an empty chat prompt
and not a life-audit questionnaire. The assistant will:

1. explain what the system can help with;
2. offer examples such as tasks, work, learning, health, finances, home and
   current projects;
3. help you select one to three useful starting points;
4. understand what you want to achieve or make easier there; and
5. agree on the language for stored information and summarise a minimal setup
   for your approval.

You can skip questions or change the setup later. Mentioning an area during
onboarding does not automatically create a folder or permanently add it to the
system.

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

When the need appears, the assistant can propose adding:

- `Projects/` for finite outcomes with several steps;
- `Areas/` for ongoing responsibilities; and
- `Daily/` for an agreed plan tied to a date.

These are not requirements. The structure should grow from real use instead of
starting as a collection of empty templates.

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
