# Webflow Brand Voice — Claude Code Skill

This repo contains a skill for [Claude Code](https://claude.ai/code) that teaches Claude how Webflow writes. Once installed, you can ask Claude to write, edit, or review any content in Webflow's voice — and it'll know the rules.

---

## What is a skill?

A skill is a markdown file that gives Claude Code a set of instructions to follow. Drop it in the right folder, and Claude will use it automatically when it's relevant, or whenever you ask.

---

## Installation

**1. Copy the skill file into your project:**

```bash
your-project/
└── .claude/
    └── skills/
        └── webflow-brand-voice.md   ← copy this file here
```

That's it. Claude Code will pick it up automatically.

**2. (Optional) Copy the reference files too:**

The skill references two supporting files for deeper guidance. If you want Claude to use them, copy the `references/` folder into your project as well:

```bash
your-project/
├── .claude/
│   └── skills/
│       └── webflow-brand-voice.md
└── references/
    ├── tone-by-surface.md
    └── inclusive-language.md
```

---

## How to use it

Once the skill is installed, just ask Claude naturally. Some examples:

> "Write a LinkedIn post about our new Localization feature."

> "Edit this blog intro so it sounds more like Webflow."

> "Does this ad copy match our brand voice? What's off?"

> "Draft a support response for a customer who can't find the CMS."

You can also be explicit: **"Use Webflow's voice"**, **"write like Webflow"**, or **"check this against our brand guidelines"**.

---

## What the skill knows

| Topic | What's covered |
|---|---|
| Brand personality | The wise mentor — knowledgeable, empowering, down-to-earth, bold |
| Voice vs. tone | Voice is constant; tone shifts by audience, context, and surface |
| Grammar rules | Active voice, contractions, Oxford comma, sentence case, and more |
| Words we don't use | Specific phrases to avoid, and what to say instead |
| Inclusive language | Ableist, gendered, racist, and culturally appropriative terms to avoid |
| Punctuation | Em dashes, ellipses, exclamation points — when and how |
| Capitalization | Sentence case, product names, ALL CAPS rules |
| Emoji | When to use them (sparingly) and when not to |
| AEO (blog content) | How to structure posts for AI-powered search |

---

## Files in this repo

```
wf-brand-voice/
├── .claude/
│   └── skills/
│       └── webflow-brand-voice.md   ← the skill
├── references/
│   ├── tone-by-surface.md           ← tone guidance for web, social, ads, support, etc.
│   └── inclusive-language.md        ← full inclusive language tables
└── README.md
```

---

## Updating the guidelines

Everything lives in plain markdown files — no build process, no dependencies.

- **Brand voice changes** → edit `.claude/skills/webflow-brand-voice.md`
- **Tone by surface** → edit `references/tone-by-surface.md`
- **Inclusive language** → edit `references/inclusive-language.md`
