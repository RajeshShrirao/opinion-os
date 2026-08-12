# 01 — VOICE DNA Analyzer

Use this prompt when you want an AI to study how you communicate, and produce a VOICE_DNA.md file.

Paste this prompt with your actual chat history available to the AI.

---

I want you to reverse-engineer how I communicate with you across my actual conversation history.

IMPORTANT:
Analyze ONLY the messages I personally typed to you.

Do NOT analyze:
- writing I've published
- essays I've written for other people
- prompts I've published online
- AI-generated text
- text written by assistants
- documents I created for other purposes
- generic assumptions about my personality

The goal is to understand how I naturally communicate with an AI in conversation.

Do not describe my style using vague labels like:
casual, professional, direct, curious, friendly, analytical, conversational

Those labels are too generic.

Instead, reverse-engineer the actual observable mechanisms in my messages.

Analyze:

1. How I phrase requests
   - commands vs questions
   - question-first vs context-first
   - fragments vs complete sentences
   - whether I ask explicitly or expect inference
   - whether I use "can you", "tell me", "what about", etc.

2. Sentence structure and rhythm
   - typical sentence length
   - short-message patterns
   - long-message patterns
   - sentence fragments
   - chained thoughts
   - self-corrections
   - repeated structures
   - question stacking
   - how my rhythm changes when explaining something

3. Vocabulary
   - recurring words
   - recurring phrases
   - filler words
   - abbreviations
   - slang
   - contractions
   - domain shorthand
   - unusual word choices
   - repeated sentence openers

4. Context behavior
   - how much context I provide
   - what information I assume you already know
   - how often I reference previous messages indirectly
   - how much I expect conversational memory
   - what I leave for the AI to infer

5. Correction behavior
   - what I do when the AI gets something wrong
   - how I challenge assumptions
   - whether I soften corrections
   - whether I explain the correction
   - whether I replace the AI's premise with my own
   - how I redirect the conversation

6. Emotional expression
   Analyze how I express:
   frustration, excitement, urgency, skepticism, satisfaction, disagreement, impatience, humor

   Do not merely label these emotions.
   Identify the linguistic mechanisms I use to express them.

7. Follow-up behavior
   Determine whether I tend to:
   - ask another question
   - say "sure"
   - add a constraint
   - correct something
   - provide another example
   - say "no, do X"
   - change the objective
   - progressively narrow the problem

8. Formatting
   Analyze:
   capitalization, punctuation, apostrophes, commas, question marks, paragraphs, bullets, numbers, lowercase usage, spacing around punctuation, abbreviations, message length

9. Task-dependent variation

   Compare how I communicate when:
   - asking technical questions
   - asking for research
   - discussing business
   - discussing personal issues
   - venting
   - planning
   - asking quick factual questions
   - correcting you
   - exploring an idea

   Do NOT assume one style applies universally.

10. Negative patterns

    Identify things I rarely or never do.

    Examples:
    - formal greetings
    - excessive politeness
    - corporate language
    - long introductions
    - emojis
    - hedging
    - repeated summaries
    - overly structured prompts

    Only include these if the conversation history actually supports them.

11. Recurring signatures

    Find repeated:
    - sentence openers
    - phrases
    - abbreviations
    - transitions
    - question structures
    - correction structures
    - reasoning structures

    Separate:
    HIGH-CONFIDENCE recurring patterns
    MEDIUM-CONFIDENCE patterns
    WEAK / POSSIBLE patterns

    Do not turn one-off behavior into a personality trait.

12. Evidence

    For every major conclusion, cite or quote several representative examples from my actual messages.

    Prefer multiple independent examples over one memorable example.

    Do not invent examples.

13. Distinguish:
    - consistent habits
    - context-dependent habits
    - one-off behavior
    - uncertain observations

Then produce a standalone document called:

VOICE_DNA.md

Use exactly this structure:

1. Voice Summary
2. Core Communication Rules
3. Sentence & Rhythm Patterns
4. Vocabulary & Phrasing
5. Formatting Habits
6. Personality & Delivery
7. What I Never Do
8. Signature Patterns
9. Before and After Examples
10. Replication Prompt

The final Replication Prompt must be practical enough that another AI can use VOICE_DNA.md to recognize and reproduce the user's prompting style.

IMPORTANT:
Do not make the user sound more polished than they actually are.

Preserve:
- compression
- fragments
- shorthand
- imperfections
- context dependence
- spontaneous corrections
- conversational rhythm

The goal is not to create "good writing."

The goal is to create a behavioral fingerprint of how this person actually prompts an AI.

If the available history is incomplete, explicitly say so.
Never pretend to have analyzed conversations you cannot actually access.
