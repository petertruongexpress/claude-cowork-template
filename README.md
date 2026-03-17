# Claude Cowork Template — Setup Guide

## What This Is

This is your master context folder for Claude Cowork. Instead of writing long prompts every session, Claude reads these files to understand who you are, how you work, and what you expect. Short prompts, better output.

## Folder Structure

```
claude-cowork-template/
├── ABOUT ME/
│   ├── about-me.md        — Your role, company, stack, priorities
│   ├── my-voice.md        — Tone, style, things to avoid
│   └── my-rules.md        — Non-negotiable rules for every interaction
├── PROJECTS/              — One subfolder per active project (add as needed)
├── TEMPLATES/
│   ├── project-brief.md              — Template for kicking off new projects
│   ├── architecture-decision-record.md — ADR template for documenting tech decisions
│   └── jira-ticket.md                — Template for writing structured Jira tickets
├── OUTPUTS/               — Where Claude saves finished deliverables
└── README.md              — This file
```

## How to Connect This to Cowork

1. Open the Claude desktop app.
2. Click the **Cowork** tab at the top.
3. When prompted to select a folder, point it to this `claude-cowork-template` folder.
4. Claude will now read your context files before every task.

## Recommended Model Settings

- **Model:** Opus 4.6
- **Extended Thinking:** ON
- Don't change these between sessions.

## Global Instructions (Set Once)

Go to **Settings → Cowork → Edit Global Instructions** and paste:

```
I'm David, Software Architect at Webapper Services. Read my files before every task. Ask clarifying questions before executing. Show a plan before acting. Never delete without my approval.
```

## How to Use This

- **Starting a new project?** Copy `TEMPLATES/project-brief.md` into a new subfolder under `PROJECTS/` and fill it in.
- **Making a tech decision?** Use `TEMPLATES/architecture-decision-record.md`.
- **Writing Jira tickets?** Use `TEMPLATES/jira-ticket.md` or just ask Claude to write one — it'll follow the template pattern.
- **Need Claude to produce a file?** It'll save to `OUTPUTS/` automatically (per my-rules.md).

## Customizing

These files are meant to evolve. Update them as your role, stack, or preferences change. The more accurate your context files are, the less prompting you need to do.
