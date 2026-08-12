# Opinion-os — public

This is the public, stripped version of Opinion-os.

It contains the prompts and templates for building your own Personal AI DNA. It does not contain anyone's actual DNA files.

## The idea

Personal AI DNA has two separate modules:

- **VOICE DNA** — how you communicate with an AI
- **OPINION DNA** — how you reason through claims and arrive at conclusions

These are different layers. The important thing is not to merge them too early.

Your Voice DNA says how you phrase requests, how you use fragments and shorthand, how you correct the AI, how your rhythm changes by task.

Your Opinion DNA says what evidence you trust, how you handle uncertainty, how you change your mind, what would make you reject an argument.

How someone talks and how someone decides what is true are different things. Keep them separate.

## The flow

```text
                 ┌─────────────────┐
                 │  CHAT HISTORY   │
                 └────────┬────────┘
                          │
                          ▼
                 ┌─────────────────┐
                 │  VOICE ANALYSIS │
                 └────────┬────────┘
                          │
                          ▼
                    VOICE_DNA.md
                          │
                          ▼
                 ┌─────────────────┐
                 │ ADAPTIVE        │
                 │ OPINION         │
                 │ INTERVIEW       │
                 └────────┬────────┘
                          │
                          ▼
                   OPINION_DNA.md
                          │
                 ┌────────┴────────┐
                 │                 │
                 ▼                 ▼
             VOICE           REASONING
                 │                 │
                 └────────┬────────┘
                          ▼
                PERSONAL_AI_OS.md
                          │
                          ▼
                 RUNTIME PROMPT
                          │
                          ▼
                     OTHER AI
```

## What's in this repo

```text
opinion-os/
├── README.md
├── concept.md
├── SECURITY.md
├── SKILL.md                 # reference — how to load the system as a skill
├── 00-ONE-CLICK.md         # the full 5-phase build in one prompt
├── 01-VOICE-DNA-ANALYZER.md
├── 02-OPINION-DNA-INTERVIEW.md
├── 03-ADAPTIVE-INTERVIEW.md
├── 04-PERSONAL-OS-SYNTHESIS.md
├── 05-RUNTIME-PROMPT.md
├── 06-VOICE-UPDATE.md
├── 07-OPINION-UPDATE.md
├── templates/
│   ├── VOICE_DNA.md
│   ├── OPINION_DNA.md
│   └── PERSONAL_AI_OS.md
└── examples/
```

- `01` through `07` — the prompts. Use them in order, or skip to the one you need.
- `templates/` — the empty structures you fill in after running the analyzer and interview.
- `concept.md` — the two-module model and the flow, explained.
- `SECURITY.md` — what never goes public.
- `SKILL.md` — a reference showing how the system is packaged as a skill, and how to load it.

`examples/` is empty on purpose. There is no sample profile here. A fictional example would undercut the one rule the system itself teaches: don't invent beliefs. Build your own using the prompts.

## How to build your own

1. Build your private VOICE_DNA.md using prompt `01`. Feed it your actual chat history — only the messages you typed, not AI output, not published writing.
2. Build your private OPINION_DNA.md using prompts `02` and `03`. The AI interviews you one question at a time. Do not let it infer your beliefs from your writing.
3. Optionally, run `04` to combine them into a PERSONAL_AI_OS.md.
4. Use `05` as your runtime prompt — paste it into an AI's system prompt with your two DNA files.
5. When you have new history, run `06` and `07` to update without rewriting from scratch.

Keep your DNA files private. See SECURITY.md.

## The one-click version

If you do not want to understand the architecture, use `00-ONE-CLICK.md`. It runs all five phases in one prompt:

- Phase 1 — Voice DNA from your history
- Phase 2 — Opinion DNA from an interview
- Phase 3 — Synthesis into a Personal AI OS
- Phase 4 — Runtime prompt
- Phase 5 — Safety and accuracy rules

If you want more control, run `01` through `05` in order instead. The phases are more useful on their own.

The repo also includes `06` and `07` for updating an existing profile without rewriting it from scratch.

## What the AI should do with your DNA files

When you give an AI your VOICE_DNA.md and OPINION_DNA.md, it should:

- match how you communicate, without parodying your typing
- reason in a way compatible with how you think
- not invent beliefs for you
- say when something is explicit, strong, possible, or unknown
- engage the actual argument when it disagrees
- treat corrections and follow-ups as new information

It should not:
- automatically agree
- automatically disagree
- confuse how you reason with what you believe
- make confidence stronger than the evidence supports
- force a replacement theory just because an old one failed

## Why two modules

If you collapse Voice and Opinion into one profile, the AI starts inventing beliefs for you. It takes your communication style and mistakes it for your worldview. That's the failure mode the two-module model prevents.

Voice DNA is behavioral. Opinion DNA is procedural. They are not the same file, and they should not become the same file.

## Updates

People change. VOICE_DNA.md changes slowly. OPINION_DNA.md can change more.

Use `06` and `07` to revise a profile when you have new history. Only change a stable rule when enough evidence supports it. One unusual message is not enough.

## Security

Read SECURITY.md. The short version:

- Keep your DNA files in a private repo or a private folder.
- Do not commit raw chat logs with other people's data or credentials.
- Do not commit `.env`, `config.yaml` with keys, `auth.lock`, `state.db`, or anything like that.
