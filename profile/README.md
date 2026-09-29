Markdown · README.md

# AI Skills for Notre Dame

Public Claude skills built by the [AI Enablement](https://ai.nd.edu/) team.

This repository contains reusable instruction packages developed at the University of Notre Dame's [Office of Information Technology](https://oit.nd.edu/). These skills extend Claude's capabilities for Notre Dame workflows, from design systems to brand guidance to specialized processes.

---

## What Are Claude Skills?

Claude skills are instruction modules that teach Claude how to handle specialized tasks. Each skill is self-contained and portable—you install it once, then reference it by name in any Claude conversation.

A skill might encode:

- Design systems and visual guidelines
- Your organization's processes and terminology
- Domain expertise or best practices
- Standards for content or communication

Once installed, skills work automatically across Claude's chat, automation, and coding applications—giving you consistent, context-aware assistance everywhere you use Claude.

---

## Available Skills

**[nd-web-theme](./nd-web-theme/)** — Design and content guidance for Notre Dame's web platform\
Guidelines for building artifacts and content aligned with NDT4, Conductor, and ND's visual brand.

**[AI-ND Brand](./ai-nd-brand/)** — Messaging and brand guidelines for AI@ND\
Voice, visual identity, and communication standards for AI@ND content and initiatives.

More skills in development. [Watch this repository](https://github.com/OIT-AI-Skills) for updates.

---

## Get Started

### Install a Skill

**In Claude.ai:**

1. Go to **Settings** → **Skills**
2. Click **Add skill**
3. Paste: `https://github.com/OIT-AI-Skills/[skill-name]`
4. Follow the prompts

**From Claude Code:**

```bash
claude skills add https://github.com/OIT-AI-Skills/[skill-name]
```

See each skill's `README.md` for full details.

### Use a Skill in Claude

Once installed, reference the skill by name:

> "Use the **nd-web-theme** skill when you design this artifact."

> "Apply the **AI-ND Brand** guidelines to this content."

Claude automatically loads the skill's instructions when you mention it.

---

## Share Your Ideas

### Have a Skill Idea?

If there's a workflow, process, or capability that would benefit the Notre Dame community, we want to hear about it.

### Want to Contribute?

If you've built a skill that could help others at Notre Dame, we'd welcome a conversation about adding it here.

### Get in Touch

Email **[ai@nd.edu](mailto:ai@nd.edu)** with:

- **Skill requests** — Describe the workflow or task you'd like to automate or streamline
- **Contributions** — Share what you've built and how others might use it
- **Questions** — Ask about skill development or how to use existing skills

---

## Learn More

**AI Enablement at Notre Dame** helps faculty, staff, and students work with AI tools effectively.

- [ai.nd.edu](https://ai.nd.edu/) — AI@ND initiative overview
- [oit.nd.edu](https://oit.nd.edu/) — Office of Information Technology
- [ai@nd.edu](mailto:ai@nd.edu) — Get in touch
