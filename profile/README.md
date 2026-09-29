Markdown · README.md

# Agent Skills for Notre Dame

Open, portable skills that teach AI agents how to work the Notre Dame way.

Built and maintained by **AI Enablement** in the [Office of Information Technology](https://oit.nd.edu/) at the University of Notre Dame, and shared publicly for anyone in the ND community — and beyond — to use.

---

## What Is an Agent Skill?

A skill is a folder of instructions that an AI agent reads when it needs them. The common convention is a `SKILL.md` file — a short description of when the skill applies, followed by the guidance itself — alongside any reference documents, templates, or scripts the agent uses as it works. Some skills ship in a specific tool's instruction format instead; the idea is the same either way.

Because it's all plain Markdown, a skill travels. The same guidance can serve Claude, ChatGPT, Gemini, Copilot, Cursor, and other agent tools — what changes is where the folder goes and what the tool calls it.

Skills are useful when an agent needs context it can't infer:

- **Institutional knowledge** — our systems, our conventions, the names we use for things
- **Standards and process** — how we brand things, how we review code, how we publish
- **Domain expertise** — the accumulated judgment that separates an acceptable answer from a good one

Without a skill, you re-explain the same context in every conversation. With one, the agent already knows.

---

## Skills in This Organization

Two pairs, each covering one side of a related problem.

### Notre Dame Brand and Web

**[notre-dame-brand](https://github.com/OIT-AI-Skills/notre-dame-brand)** — Applies the University's masterbrand standards to materials an agent produces: ND Blue and Bright Gold, the Galaxie Polaris typographic system, Academic Mark placement, and brand voice. Built for slides, posters, flyers, social graphics, and donor and event communications. Treats [onmessage.nd.edu](https://onmessage.nd.edu/) as the source of truth, and defers to Notre Dame Creative on stationery, merchandise, athletics co-branding, and custom unit lockups.

**[nd-web-theme-conductor](https://github.com/OIT-AI-Skills/nd-web-theme-conductor)** — Creates and styles content for Conductor sites running the Notre Dame Web Theme v4. The agent composes paste-ready content HTML from official theme components rather than inventing its own markup, so pages match what ND's web team builds and survive theme updates.

Use the brand skill for materials and the theme skill for anything web-bound; the two hand off to each other at that line.

### AI-Assisted Development

**[vibe-coding-discipline](https://github.com/OIT-AI-Skills/vibe-coding-discipline)** — Engineering practices for coding agents: branching and pull requests, test coverage, and documentation — the habits that keep agent-assisted work reviewable and maintainable.

**[vibe-coding-security-scanner](https://github.com/OIT-AI-Skills/vibe-coding-security-scanner)** — Reviews AI-generated code for the gaps automated scanners tend to miss: data exfiltration paths, secrets handling, and privilege escalation, with language-specific rules for Ruby/Rails and Python and extensible templates for others. Output is deterministic, machine-parseable Markdown, so it runs interactively in an editor or as a step in CI.

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
| GitHub Copilot / VS Code | The instruction files go under `.github/` in the repo you're working in |
| Other agents | Check your tool's documentation for its skills or instructions directory |

Support for the skills format is expanding quickly, and each tool names things a little differently. Each repository's own README has current, specific instructions — start there if the table above doesn't match what you see.

---

## Using a Skill

Once installed, most agents load a skill on their own when the work calls for it — that's what the description at the top of `SKILL.md` is for. You can also ask directly:

> Use the nd-web-theme-conductor skill to build a landing page for our new service.

> Make this slide deck follow the Notre Dame brand skill.

> Follow vibe-coding-discipline on this branch, then run the security scanner over what you wrote.

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
