# Write Better

A Claude Code skill that acts as a writing editor, helping refine drafts into clear, concise writing while preserving the writer's voice.

## Usage

Invoke the skill with `/write-better` followed by (or alongside) your draft text.

## How It Works

The skill operates in three modes depending on where your draft is:

- **Green stump** (early): Helps structure scattered thoughts, find the core argument, identify gaps in thinking
- **Rough draft** (middle): Tightens structure, cuts digressions, strengthens weak sections
- **Polished draft** (late): Line-level editing for clarity, concision, and rhythm

## Voice Profile

On first use, the skill will ask for a writing sample to create a voice profile stored at `.claude/writing-voice-profile.md`. This ensures edits preserve your natural voice rather than producing generic AI-sounding output.

## Principles

Built on writing advice from Paul Graham, George Orwell, William Zinsser, Wes Kao, Shreyas Doshi, Jeff Bezos, Steven Pinker, and other clear thinkers. Key principles:

- Clarity above all -- clear writing comes from clear thinking
- Cut ruthlessly -- most drafts can lose 30-50% without losing meaning
- Have a point of view -- writing without a stance says nothing useful
- Lead with the conclusion (BLUF) -- respect the reader's time
- Narrative over bullet points -- full sentences force logical rigor
- Preserve the writer's voice -- sharpen, don't replace
