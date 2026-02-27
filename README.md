# wf-brand-voice

A Claude Code skill that applies Webflow's brand voice, tone, and style guidelines to any content you write, edit, or review.

## What this skill does

The `webflow-brand-voice` skill gives Claude a deep understanding of how Webflow communicates — the personality, the rules, the things we never say — so it can write, edit, or review content that sounds unmistakably like Webflow.

Use it for:

- Marketing copy, landing pages, and ads
- Blog posts and long-form content (with AEO optimization baked in)
- UI copy and product microcopy
- Social posts (LinkedIn, X/Twitter, Instagram)
- Support responses and lifecycle emails
- Any content that needs a brand gut-check

## How to install

This skill is installed per-project in Claude Code. To use it, clone or copy this repository into your project (or point Claude Code at this repo as a skill source).

### Option 1: Copy the skill file directly

Copy `.claude/skills/webflow-brand-voice.md` into the `.claude/skills/` directory of any project where you want the skill available.

```
your-project/
└── .claude/
    └── skills/
        └── webflow-brand-voice.md
```

If you also want the reference files (inclusive language, tone by surface), copy the `references/` folder alongside the skill:

```
your-project/
├── .claude/
│   └── skills/
│       └── webflow-brand-voice.md
└── references/
    ├── tone-by-surface.md
    └── inclusive-language.md
```

### Option 2: Use this repo as-is

Clone this repo and work from it directly. The skill is already in the right place.

```bash
git clone <this-repo-url>
```

## How to use

Once installed, Claude will automatically apply the brand voice skill whenever the context makes it relevant. You can also invoke it explicitly:

**Write new content:**
> "Write a LinkedIn post announcing our new Localization feature. Use Webflow's voice."

**Edit existing content:**
> "Edit this blog intro for brand alignment."

**Review for brand fit:**
> "Does this ad copy match Webflow's voice? Flag anything that's off."

**Trigger phrases that activate the skill:**
- "Write like Webflow"
- "Use Webflow's voice"
- "Check brand guidelines"
- "Draft content for Webflow"

## What's in the skill

The skill encodes Webflow's full brand voice system:

| Section | What it covers |
|---|---|
| **Brand personality** | The wise mentor — knowledgeable, empowering, down-to-earth, bold |
| **Voice dimensions** | The four core traits and what each one means in practice |
| **Voice vs. tone** | How tone shifts by audience, context, and surface |
| **Grammar rules** | Active voice, contractions, Oxford comma, sentence case, and more |
| **"Don't say" list** | The specific phrases and words we never use, and what to say instead |
| **Inclusive language** | Pronouns, ableist terms, gendered language, racial/cultural language |
| **Punctuation** | Em dashes, en dashes, ellipses, exclamation points — when and how |
| **Capitalization** | Sentence case rules, product name capitalization, ALL CAPS policy |
| **Emoji** | When to use them and when not to |
| **AEO optimization** | How to structure blog content for AI-powered search |

## Reference files

The skill points to two supporting reference files. These are stubs — populate them with your full guidelines.

| File | Purpose |
|---|---|
| `references/tone-by-surface.md` | Tone guidance broken down by content surface (web, social, ads, support, etc.) |
| `references/inclusive-language.md` | Full inclusive language tables for ableist, gendered, racial, and cultural terms |

## Repo structure

```
wf-brand-voice/
├── .claude/
│   └── skills/
│       └── webflow-brand-voice.md   ← the skill
├── references/
│   ├── tone-by-surface.md           ← tone guidance by surface (expand me)
│   └── inclusive-language.md        ← inclusive language tables (expand me)
└── README.md
```

## Maintaining this skill

When Webflow's brand guidelines change, update `.claude/skills/webflow-brand-voice.md` directly. The skill is a single markdown file — no build step, no dependencies.

For surface-specific tone updates, edit `references/tone-by-surface.md`.
For inclusive language updates, edit `references/inclusive-language.md`.
