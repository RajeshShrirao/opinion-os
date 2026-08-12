# SKILL.md — Reference

This is a reference showing how the Opinion-os writing system is packaged as a Hermes skill, and how you can load it to write or calibrate text in your own voice.

This file is part of the public, stripped repo. It does NOT include anyone's personal DNA files.

## What this skill is

Opinion-os is a writing system made of:

- **VOICE_DNA.md** — how the writing sounds (in your private repo)
- **OPINION_DNA.md** — how opinions are formed (in your private repo)
- **AI_WRITING_BLACKLIST.md** — the banned list of AI-writing habits
- **humanizer** — a sub-skill that calibrates a draft to a voice and opinion style
- **stop-slop** — a sub-skill that kills obvious AI-writing habits

The DNA files are personal. Keep them in your private repo.

## How to load it

If you have opinion-os installed as a skill, load it when you are about to do any writing task:

- Load `opinion-os` for the full system
- Load `opinion-os-humanizer` when you want to calibrate a draft to a voice
- Load `opinion-os-stop-slop` when you want a focused cleanup

If you do not have opinion-os installed, build your own private version using the prompts in this repo, put the skill tree in your private repo, and load it from there.

## How to use it to write in your voice

1. Build your private VOICE_DNA.md and OPINION_DNA.md using the prompts in this repo.
2. Package them into a skill tree like the one in the private repo.
3. Load the skill before writing.
4. Run the blacklist as the final pass.

The skill does not invent your voice for you. You have to build the DNA files first.

## Files in the skill tree

- `SKILL.md` — entry point
- `VOICE_DNA.md` — your private voice profile
- `OPINION_DNA.md` — your private opinion profile
- `WRITING_SYSTEM.md` — the meta-instruction
- `AI_WRITING_BLACKLIST.md` — the banned list
- `opinion-os-humanizer/SKILL.md` — sub-skill
- `opinion-os-stop-slop/SKILL.md` — sub-skill

Only the SKILL.md, WRITING_SYSTEM.md, AI_WRITING_BLACKLIST.md, and the sub-skill SKILL.md files are safe to publish. The DNA files are not.
