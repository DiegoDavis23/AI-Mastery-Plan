# Day 3: Prompt Engineering Mastery

> Atomic Digital — AI Mastery Learning Plan

---

## What is a Prompt?

A prompt is just the instructions you give to an AI. The better your instructions, the better the output. Think of it like briefing a freelancer — vague brief = vague work.

---

## The 3 Key Concepts

### 1. System Prompts

A **system prompt** is a hidden instruction that sets the AI's personality, rules, and context *before* the user says anything. The user never sees it, but it controls how the AI behaves.

**Without system prompt:**

> "Write me a meta description" → Generic, could be any style

**With system prompt:**

> *System: You are a senior SEO specialist at Atomic Digital. You write concise, click-worthy meta descriptions under 155 characters that include the target keyword naturally.*
>
> "Write me a meta description for a page about AI marketing" → Way more specific and on-brand

Think of the system prompt as the AI's **job description**. You write it once, and every response follows those rules.

---

### 2. Temperature

**Temperature** controls how creative vs predictable the AI is. It's a number from 0 to 1.

| Temperature | Behavior | Best For |
|---|---|---|
| **0** | Deterministic, same answer every time | Code, data extraction, factual answers |
| **0.3 - 0.5** | Mostly consistent with slight variation | SEO meta descriptions, email copy |
| **0.7 - 0.8** | Creative and varied | Blog posts, brainstorming, ad copy |
| **1.0** | Maximum creativity, sometimes wild | Brainstorming, creative writing |

**Rule of thumb:** If there's a "right answer," use low temperature. If you want ideas, go higher.

---

### 3. Structured Outputs

Instead of getting a wall of text back, you can tell Claude to respond in a **specific format** — usually JSON. This is huge for building tools because you can feed the output directly into your code.

**Without structure:**

> "Give me 3 blog title ideas" → You get a paragraph with bullets

**With structure:**

```
Give me 3 blog title ideas. Respond in this exact JSON format:
{
  "titles": [
    { "title": "...", "target_keyword": "...", "search_intent": "..." }
  ]
}
```

Now you get clean data you can use programmatically.

---

## Putting It All Together

A great prompt has **5 elements:**

1. **Role** — Who is the AI? (system prompt)
2. **Context** — What's the situation?
3. **Task** — What exactly do you want?
4. **Format** — How should the output look?
5. **Constraints** — Any rules or limits?

**Example:**

```
Role: You are an SEO copywriter at Atomic Digital.
Context: Our client sells organic skincare products.
Task: Write a meta description for their homepage.
Format: One line, under 155 characters.
Constraints: Include the keyword "organic skincare",
use active voice, include a call to action.
```

---

## Key Takeaways

- **System prompts** = the AI's job description. Set it once, every response follows it.
- **Temperature** = creativity dial. Low for accuracy, high for ideas.
- **Structured outputs** = get JSON/formatted data instead of paragraphs. Essential for building tools.
- **Every good prompt** has: Role, Context, Task, Format, and Constraints.
