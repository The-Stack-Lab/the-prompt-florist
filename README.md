# Prompt Florist 🌸

Turn vague ideas into precise, art-directed prompts that get results.

Prompt Florist is a Claude Code Skill that cultivates project context, learns from feedback, and compounds taste over time.

---

## What It Does

- Takes rough prompts and expands them into detailed "Bouquets"
- Learns your project's brand, constraints, and visual taste
- Stores learning in project files (memory.md, vase.md)
- Improves output quality through continuous feedback
- Acts like a junior design director who gets better over time

---

## Installation

### Prerequisites
- Claude Code CLI installed
- Active Claude project

### Install Steps

1. Clone this repo:
```bash
   git clone https://github.com/The-Stack-Lab/the-prompt-florist.git
```

2. Copy the Skills to your project:
```bash
   cp -r the-prompt-florist/.claude/skills/* YOUR_PROJECT/.claude/skills/
```

3. Navigate to your project and start Claude Code

4. Use the Skill:
```bash
   Use Prompt Florist to improve this prompt: [your rough idea]
```

---

## First Run

On first use, Prompt Florist will guide you through:

1. **Project Charter** - Define purpose, constraints, desired outcomes
2. **Brand Ingestion** - Add visual guidelines, colors, typography
3. **Visual Examples** - Upload reference designs (the "Vase")
4. **Memory Initialization** - Set up learning log

After setup, it's ready to hydrate prompts.

---

## How It Works

### Input
"Build a homepage hero for a SaaS product"

### Output: Prompt Bouquet
1. Refined Intent
2. Assumptions (made explicit)
3. Design & UX Constraints
4. Visual Direction
5. Explicit Build Prompt (copy/paste ready)
6. Do Not List (anti-patterns)

### Feedback Loop
After each bouquet:
- Rate 1-5
- Provide feedback
- Learning gets stored in `memory.md`
- Taste principles update in `vase.md`

---

## File Structure
```
/florist/
  charter.md           # Project identity
  /brand/              # Visual guidelines
  /examples/           # Reference designs
  /knowledge/
    memory.md          # Append-only learning log
    vase.md            # Curated quality standards
```

---

## Core Concepts

**Bouquet** - A fully hydrated prompt with context, constraints, and guardrails

**Vase** - Curated record of "what good looks like"

**Memory** - Append-only log of feedback and lessons learned

**Harvest** - Periodic synthesis that validates learning and prevents drift

---

## Advanced Usage

### Harvest Command
Periodically run Harvest to:
- Synthesize accumulated learning
- Validate with user
- Reindex project knowledge
```bash
Use Harvest to synthesize what Prompt Florist has learned
```

---

## Philosophy

Prompt Florist treats prompts as design artifacts that benefit from:
- Accumulated context
- Explicit constraints
- Continuous feedback
- Compounding judgment

It's NOT:
- A one-shot generator
- A template system
- A vibe-based creative tool

---

## Contributing

Issues and pull requests welcome at:
https://github.com/The-Stack-Lab/the-prompt-florist

---

## License

TBD

---

## Author

Planted by Kyle of The Stack Lab (Stacks, Inc)