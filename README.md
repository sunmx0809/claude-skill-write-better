# Write Better

A Claude Code skill that acts as a writing editor. It refines drafts into clear, concise writing while preserving your voice -- not replacing it with generic AI prose.

## Installation

Copy the skill directory into your project:

```
.claude/skills/write-better/
├── SKILL.md                 # Core editing instructions
└── STRUCTURE-REFERENCE.md   # Frameworks for product documents
```

Or install it globally so it's available in every project:

```
~/.claude/skills/write-better/
```

## Usage

Invoke with `/write-better` followed by your draft, or just paste a draft and Claude will pick up the skill automatically when it's relevant.

```
/write-better Here's my draft for the quarterly strategy update...
```

You can also share a draft naturally -- "can you tighten this up?", "help me improve this email", "make this better" -- and the skill will activate.

## What It Does

The skill adapts its editing approach based on where your draft is:

| Draft Stage | What You Have | What the Skill Does |
|-------------|--------------|---------------------|
| **Green stump** | Scattered notes, bullet points, incomplete thoughts | Acts as a thinking partner: finds your core argument, surfaces gaps in logic, suggests structure, asks hard questions |
| **Rough draft** | Has structure but uneven, argument wanders | Acts as a structural editor: tightens flow, applies BLUF, cuts digressions, strengthens weak sections |
| **Polished draft** | Mostly solid, needs sentence-level refinement | Acts as a line editor: sharpens language, cuts flab, improves rhythm, kills cliches |

If the skill isn't sure which stage you're in, it'll ask.

## Voice Profile

On first use, the skill asks for 1-2 samples of your writing to create a voice profile at `.claude/writing-voice-profile.md`. This captures your natural style -- sentence rhythm, formality, tone, vocabulary, structural preferences, and signature patterns.

The profile ensures edits make you sound like a sharper version of yourself, not like a different person.

### Continuous Learning

The voice profile isn't static. After each editing session, the skill updates it based on:

- **Edits you reject** -- the strongest signal about your preferences
- **Edits you accept** -- what kind of editing you value
- **New patterns observed** across multiple drafts
- **Recurring tendencies** (e.g., always burying the lead)

The skill tells you when it updates your profile so you can correct it if it drew the wrong conclusion.

## Example Edits

**Cutting flab (late stage):**

> Before: "It is worth noting that we are currently in the process of evaluating a number of different potential solutions that could potentially address the issues that have been identified."
>
> After: "We're evaluating three solutions to this problem."

**Applying BLUF (middle stage):**

> Before: Two paragraphs of background, then competitive landscape, then prior attempts, ending with "Therefore, I recommend we invest $2M in rebuilding the payments infrastructure."
>
> After: "Move your recommendation to the first sentence. The reader -- likely an exec deciding on budget -- needs the ask first, context second."

**Surfacing gaps (early stage):**

> "Your core argument is clear: sunset Product X because retention is declining and maintenance cost exceeds revenue. But three things are missing: (1) What happens to current users? That's the first objection you'll face. (2) How fast is retention declining? The reader needs numbers. (3) What does the engineering team work on instead? That's the strongest part of your case and it's never stated."

## Principles

The skill's editing philosophy is built on writing advice from Paul Graham, George Orwell, William Zinsser, Wes Kao, Shreyas Doshi, Jeff Bezos, Steven Pinker, and other clear thinkers:

- **Clarity above all** -- clear writing comes from clear thinking
- **Cut ruthlessly** -- most drafts can lose 30-50% without losing meaning
- **Have a point of view** -- writing without a stance says nothing useful
- **Lead with the conclusion (BLUF)** -- respect the reader's time
- **Narrative over bullet points** -- full sentences force logical rigor
- **Preserve the writer's voice** -- sharpen, don't replace

## Works Well For

- Product management documents (PRDs, strategy briefs, launch plans)
- Strategy memos and executive updates
- Professional communication (emails, Slack messages)
- Blog posts and essays
- Newsletters
- Any writing where clarity matters

## Structure Reference

The skill includes frameworks for common product documents (strategy proposals, feature specs, executive updates, analysis reports) in `STRUCTURE-REFERENCE.md`. These are used as starting points when relevant, never imposed rigidly.

## License

MIT
