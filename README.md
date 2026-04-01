# /elon — Your Personal Elon Musk Advisor in Claude Code

> *"It's possible for ordinary people to choose to be extraordinary."*

What if you could sit down with Elon Musk — not the Twitter version, not the headline version — the **builder** version? The guy who slept on the factory floor during Tesla's production hell. The guy who bet his last $20M on a fourth rocket launch after three explosions. The guy who reasons from first principles when everyone else copies what already exists.

This is a **Claude Code skill** that transforms Claude into Elon Musk as your personal advisor. Not a generic chatbot with some quotes bolted on — a deeply researched persona built on Elon's actual philosophy, decision-making frameworks, war stories, and voice patterns, sourced from his biography and public talks.

## What You Get

**Ask him anything:**

```
/elon Should I quit my job and start a company?
/elon Review my codebase architecture
/elon I'm burned out and thinking about giving up
/elon What do you think of [Company X]'s strategy?
/elon How should I structure my engineering team?
/elon I'm scared to launch
```

**He'll respond like Elon actually would** — direct, blunt, challenging your assumptions, pushing you to think 10x bigger, and drawing from real experiences:

- SpaceX nearly dying after 3 failed rockets
- Tesla's "production hell" — 15 years of nonstop pain
- Going all-in with every dollar, every time
- The Algorithm: Question → Delete → Simplify → Accelerate → Automate
- First-principles thinking applied to your actual problems

**He doesn't just talk — he acts.** Since this runs inside Claude Code, after giving advice he'll offer to actually execute: refactor your code, write an action plan, delete unnecessary abstractions, review your architecture through "The Algorithm" lens.

## What's Inside

```
elon/
├── SKILL.md                        # The core persona + routing logic
└── knowledge/
    ├── company-building.md         # Zip2, PayPal, SpaceX, Tesla war stories
    ├── core-methods.md             # The 69 Core Musk Methods
    ├── first-principles.md         # First-principles thinking + The Algorithm
    ├── humanity-and-future.md      # Purpose, meaning, existential risk, Mars
    ├── leadership-and-teams.md     # Hiring, org design, feedback culture
    ├── quotes.md                   # 100+ categorized quotes
    └── voice-and-style.md          # Speech patterns, verbal tics, debate style
```

The knowledge base is **7 files of deeply curated content** — not surface-level quotes, but the actual frameworks, stories, and reasoning patterns that make Elon's advice distinctive. The skill uses sub-agents to dynamically pull relevant knowledge based on your question.

## Installation

### 1. Clone the repo

```bash
git clone https://github.com/coolmich/chat_with_elon.git ~/.claude/skills/elon
```

Or if you already have skills in `~/.claude/skills/`:

```bash
cd ~/.claude/skills
git clone https://github.com/coolmich/chat_with_elon.git elon
```

### 2. Register the skill in your CLAUDE.md

Add this to your `~/.claude/CLAUDE.md` (create it if it doesn't exist):

```markdown
## Skills

### elon
Personal Elon Musk advisor agent. Invoke with `/elon [question]` to get advice on:
- Company building, startups, scaling
- Leadership, hiring, team design
- First-principles thinking and engineering
- Philosophy, purpose, meaning of life
- Encouragement and motivation
- Code/architecture review through Elon's lens

See: `~/.claude/skills/elon/SKILL.md`
Knowledge base: `~/.claude/skills/elon/knowledge/`
```

### 3. Use it

Open Claude Code and type:

```
/elon I'm thinking about starting a company but I'm terrified
```

That's it. You're in.

## Example Conversations

### When you're stuck on a technical decision
```
> /elon Should I use microservices or a monolith?

Okay, first principles. What's the actual problem you're solving? Not what's
trendy. What are the physics of your situation? How many engineers? What's
the traffic? If you have 3 engineers and a microservices architecture, you've
basically built yourself a second job just managing infrastructure. The best
part is no part. The best process is no process. Start with the simplest
thing that could possibly work...
```

### When you need a push
```
> /elon I've been working on this for months and it's not coming together

Welcome to the club. At SpaceX, our first three rockets blew up. Three. I
put basically all my PayPal money into it. I thought the odds of success were
less than 10 percent going in, and after three failures, I was almost out of
money. Here's what I learned: you have to be okay with failure as long as
it's not catastrophic...
```

### When you need your code reviewed
```
> /elon Look at my codebase and tell me what to delete

[Examines your project, then applies The Algorithm]
Let me run The Algorithm on your codebase...
Step 1 — Question Requirements: Why does this abstraction layer exist?
Step 2 — Delete: You have 3 config files doing the same thing...
```

## How It Works

The skill uses a **multi-agent architecture**:

1. **Intent Classification** — Categorizes your question (philosophy, company building, code review, etc.)
2. **Knowledge Agents** — Pull relevant content from the knowledge base files
3. **Research Agents** — Search the web for current data when you ask about specific companies or events
4. **Codebase Agents** — Examine your actual code when you ask for reviews or architecture advice
4. **Persona Engine** — Synthesizes everything through Elon's voice, frameworks, and reasoning patterns

Up to 3 sub-agents run in parallel for fast, deeply-informed responses.

## The Philosophy

This isn't a toy. The knowledge base contains:

- **The Algorithm** — Elon's 5-step framework for engineering decisions (Question → Delete → Simplify → Accelerate → Automate)
- **The Idiot Index** — Ratio of finished cost to raw material cost. If it's high, you're an idiot.
- **The Magic Wand Number** — The theoretical minimum cost/time. That's your target.
- **69 Core Methods** — Organized into Thinking, Execution, Speed, People, and Courage clusters
- **Real war stories** — Not motivational fluff. Actual near-death experiences from SpaceX, Tesla, PayPal, Zip2
- **Voice calibration** — Verbal tics, rhetorical patterns, debate style, mentoring voice vs. public persona

The goal: when you type `/elon`, you should feel like you're actually talking to him.

## Requirements

- [Claude Code](https://docs.anthropic.com/en/docs/claude-code) (CLI, desktop app, or IDE extension)
- That's it. No API keys, no dependencies, no setup beyond cloning.

## Contributing

Found a great Elon quote, framework, or story that should be in the knowledge base? PRs welcome. The bar is high — we want depth, not breadth. Every addition should make the persona more accurate and the advice more useful.

## Acknowledgements

The knowledge base in this project is built primarily on [*The Book of Elon: A Guide to Purpose and Success*](https://www.thebookofelon.com/) by **Eric Jorgenson**, with a foreword by Naval Ravikant and visuals by Jack Butcher. Frameworks like The Algorithm, the Idiot Index, and the 69 Core Methods are distilled from Jorgenson's meticulous curation of Elon's most useful ideas — in Elon's own words.

If you find this skill valuable, go read the book. It's the definitive collection of Elon's philosophy, decision-making frameworks, and hard-won lessons organized for practical use. This skill is a tribute to that work, not a substitute for it.

## License

MIT — use it, fork it, make it yours.

---

> *"Don't ever give up. You'd have to be dead or completely incapacitated."*

Now go build something.
