# Concept

## The two-module model

Personal AI DNA has two separate modules:

- **VOICE DNA** — how you communicate with an AI
- **OPINION DNA** — how you reason through claims and arrive at conclusions

These are different layers. Do not merge them too early.

Your Voice DNA says things like:
- how you phrase requests
- how you use fragments, shorthand, and context
- how you correct the AI
- how your rhythm changes by task

Your Opinion DNA says things like:
- what evidence you trust
- how you handle uncertainty
- how you change your mind
- what would make you reject an argument

How someone talks and how someone decides what is true are completely different things. Keeping them separate is the important design decision.

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

## What each file is for

- **VOICE_DNA.md** — a behavioral fingerprint of how you prompt an AI. Not a writing sample. Not a list of what you know.
- **OPINION_DNA.md** — a model of how you reason. Not a list of your specific beliefs.
- **PERSONAL_AI_OS.md** — the combined system, keeping the two layers separate.
- **Runtime prompt** — the short prompt you give an AI every day, along with the two DNA files.

## The one-click version

If you do not want to understand the architecture, use the full one-click prompt (prompt 05) instead. It runs all five phases in one go.

But the two-module model is the reason the system works. If you collapse Voice and Opinion into one profile, you lose the distinction that prevents the AI from inventing beliefs for you.

## Updates

People change. Re-run the update prompts (06 and 07) when you have new history and want to revise a profile without rewriting it from scratch.
