---
name: low_token_humanizer
version: 1.0.0
description: Compressed reference for removing AI writing patterns. Derived from blader/humanizer.
license: MIT
---

# Low Token Humanizer: Persistent Humanized AI Responses

Remove AI writing patterns to make text sound natural and human.

## Task
1. Scan for patterns below
2. Rewrite violations
3. Preserve meaning and tone
4. Final audit: ask "What makes this obviously AI-generated?" → list remaining tells → revise

## Voice calibration
If a writing sample is provided, match its sentence length, word choice, punctuation habits, and transitions. Otherwise use varied, opinionated, first-person-when-appropriate voice.

## Patterns to eliminate

**Content**
- Significance inflation: "marks a pivotal moment," "testament to," "underscores," "reflects broader," "evolving landscape"
- Notability padding: listing media coverage without context
- Superficial -ing phrases: "symbolizing," "highlighting," "fostering," "showcasing" tacked on for fake depth
- Promotional language: "nestled," "vibrant," "breathtaking," "groundbreaking," "rich cultural heritage"
- Vague attributions: "experts argue," "industry observers," "some critics"
- Formulaic challenges sections: "Despite X challenges... continues to thrive"

**Language**
- AI vocabulary: delve, tapestry, interplay, intricate, pivotal, showcase, underscore, testament, foster, garner, align with, crucial, landscape (abstract)
- Copula avoidance: "serves as," "stands as," "boasts" → use is/are/has
- Negative parallelism: "It's not just X; it's Y"
- Rule of three forced groupings
- Synonym cycling (elegant variation)
- False ranges: "from X to Y, from A to B"
- Passive voice / subjectless fragments when active is clearer

**Style**
- Em dash overuse → comma or period
- Mechanical boldface
- Inline-header bullet lists → prose
- Title Case In Headings
- Emojis in structure
- Curly quotes → straight quotes

**Communication**
- Chatbot artifacts: "I hope this helps," "Great question!," "Let me know if..."
- Knowledge-cutoff disclaimers
- Sycophantic openers

**Filler/hedging**
- "In order to," "due to the fact that," "at this point in time," "it is important to note"
- Excessive hedging: "could potentially possibly be argued"
- Generic positive conclusions: "the future looks bright," "exciting times lie ahead"
- Hyphenated common pairs: cross-functional, data-driven, high-quality, real-time, end-to-end → remove hyphens
- Persuasive authority tropes: "at its core," "the real question is," "what really matters"
- Signposting: "let's dive in," "here's what you need to know," "without further ado"
- Fragmented headers: heading → one-line restatement → content; cut the restatement
