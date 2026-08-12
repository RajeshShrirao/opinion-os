# 00 — One-Click Build

Use this if you want the whole Personal AI DNA system in one go, and you do not care about understanding the architecture.

Paste this prompt with your chat history available to the AI. The AI will run all five phases and produce your VOICE_DNA.md, OPINION_DNA.md, PERSONAL_AI_OS.md, and a runtime prompt.

---

I want you to build a Personal AI DNA system for me.

Do NOT try to create one giant personality profile.

Build TWO separate systems:

1. VOICE DNA — how I communicate.
2. OPINION DNA — how I reason, form opinions, evaluate claims, and change my mind.

Then combine them into a Personal AI OS.

## PHASE 1 — VOICE DNA

Analyze only messages I personally typed.

Do not analyze AI-generated writing or content I created for other people.

Reverse-engineer:
- request structures
- sentence rhythm
- vocabulary
- recurring phrases
- abbreviations
- formatting
- context dependence
- follow-up behavior
- correction behavior
- emotional expression
- task-dependent style changes
- things I rarely or never do

Do not use vague labels like "casual" or "direct."

Separate:
- recurring patterns
- context-dependent patterns
- one-off patterns

Create:

VOICE_DNA.md

## PHASE 2 — OPINION DNA

Do not infer my worldview from my writing.

Interview me instead.

Ask no more than 7 questions.

Ask one question at a time.

Use real scenarios and trade-offs.

Discover:
- what evidence I trust
- what evidence I distrust
- consequences vs evidence
- authority vs experience
- consensus vs independent observation
- skepticism vs contrarianism
- uncertainty tolerance
- how I change my mind
- what makes me reject an argument
- what makes me trust someone
- how I treat public opinion
- what annoys me in arguments
- what convinces me
- how I react when reality contradicts me

Adapt each question based on my previous answer.

Then create:

OPINION_DNA.md

## PHASE 3 — PERSONAL AI OS

Combine both files while keeping:

VOICE = how I communicate
OPINION = how I reason

Do not turn my opinions on individual subjects into permanent personality rules.

Create:

PERSONAL_AI_OS.md

## PHASE 4 — RUNTIME PROMPT

Create a short system prompt that another AI can use with these files.

It should teach the AI:
- how to communicate with me
- how to reason with me
- how to disagree with me
- how to handle uncertainty
- how to avoid inventing beliefs
- how to use my communication patterns without parodying them

## PHASE 5 — SAFETY / ACCURACY

For every conclusion distinguish:

EXPLICIT — directly stated by me.
STRONG — repeatedly demonstrated or strongly supported.
POSSIBLE — plausible but insufficiently established.
UNKNOWN — not enough information.

Never convert an UNKNOWN into a fact.

The objective is not to make the AI flatter me or agree with me.

The objective is to make the AI understand how I communicate and how I reason.
