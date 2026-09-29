Markdown · README.md

# Agent Skills for Notre Dame

Open, portable skills that teach AI agents how to work the Notre Dame way.

Built and maintained by **AI Enablement** in the [Office of Information Technology](https://oit.nd.edu/) at the University of Notre Dame, and shared publicly for anyone in the ND community — and beyond — to use.

---

## What Is an Agent Skill?

A skill is a folder of instructions that an AI agent reads when it needs them. At minimum it's a single `SKILL.md` file: a short description of when the skill applies, followed by the guidance itself. Skills can also carry reference documents, templates, and scripts the agent uses as it works.

The format is plain Markdown, which makes it portable. The same skill works in Claude, ChatGPT, Gemini, Copilot, Cursor, and other agent tools — the only thing that changes is where you put the folder.

Skills are useful when an agent needs context it can't infer:

- **Institutional knowledge** — our systems, our conventions, the names we use for things
- **Standards and process** — how we brand things, how we review code, how we publish
- **Domain expertise** — the accumulated judgment that separates an acceptable answer from a good one

Without a skill, you re-explain the same context in every conversation. With one, the agent already knows.

---

## Skills in This Organization

### [nd-web-theme-conductor](https://github.com/OIT-AI-Skills/nd-web-theme-conductor)

Creates and styles content for Conductor websites running the Notre Dame Web Theme v4. The agent composes paste-ready content HTML using official theme components instead of inventing its own markup — so the result matches pages built by ND's web team and survives theme updates.

### [vibe-coding-discipline](https://github.com/OIT-AI-Skills/vibe-coding-discipline)

Engineering practices for coding agents: branching and pull requests, test coverage, documentation, and the habits that keep agent-assisted work reviewable and maintainable.

More skills are in development.

---

## Installing a Skill

Every skill here is a self-contained folder, so installation is the same three ideas everywhere: get the folder, put it where your agent looks for skills, restart or reload.

**Get the folder**

```bash
git clone https://github.com/OIT-AI-Skills/nd-web-theme-conductor.git
```

Or download the ZIP from the repository's green **Code** button.

**Put it where your agent looks**

| Tool | Location |
| --- | --- |
| Claude Code | `~/.claude/skills/<skill-name>/` for personal use, or `.claude/skills/<skill-name>/` to share with a repo |
| Claude (web and desktop) | Upload the folder as a skill in **Settings → Capabilities** |
| Other agents | Check your tool's documentation for its skills or instructions directory |

Support for the skills format is expanding quickly, and each tool names things a little differently. Each repository's own README has current, specific instructions — start there if the table above doesn't match what you see.

---

## Using a Skill

Once installed, most agents load a skill on their own when the work calls for it — that's what the description at the top of `SKILL.md` is for. You can also ask directly:

> Use the nd-web-theme-conductor skill to build a landing page for our new service.

> Follow vibe-coding-discipline on this branch.

---

## Request or Contribute a Skill

**Have an idea?** If there's a workflow, standard, or body of knowledge at Notre Dame that agents keep getting wrong, that's a good candidate for a skill. Tell us what you'd want it to handle.

**Built something?** If you've written a skill that would help other people at Notre Dame, we'd like to see it. We can help refine it, review it, and publish it here.

**Not sure where to start?** Ask. Part of our job is helping people figure out whether a skill is the right tool for the problem.

Email **[ai@nd.edu](mailto:ai@nd.edu)**.

---

## About AI Enablement

AI Enablement helps faculty and staff across Notre Dame adopt AI tools with confidence — through training, internal tooling, and practical guidance grounded in how the University actually works.

[ai.nd.edu](https://ai.nd.edu/) · [oit.nd.edu](https://oit.nd.edu/) · [ai@nd.edu](mailto:ai@nd.edu)
