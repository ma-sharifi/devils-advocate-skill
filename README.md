# devils-advocate

A Claude Code skill that challenges, stress-tests, and pressure-tests a design,
architecture, technical plan, or decision *before* it gets committed.

It plays the role of the smart, relentless colleague who refuses to let a weak
decision slide — attacking the design, never the designer — so the decision
comes out stronger.

## What it does

When you ask Claude to "challenge this", "poke holes in this", "red-team my
design", "play devil's advocate", or "tell me what I'm missing" — or when you
present a design that seems to have gone unchallenged — the skill works through:

1. **Steelman first** — restate the design in its strongest form.
2. **Open the option space** — surface genuinely different alternatives.
3. **Hunt the failure modes** — where it breaks under load, scale, time, and abuse.
4. **Surface the trade-off** — what it optimizes for and what it sacrifices.
5. **Test reversibility** — how costly it is to be wrong here.
6. **Land the one thing** — the single highest-leverage thing to reconsider.

It calibrates intensity to stakes: hard press on architecture, data models, and
security boundaries; a light touch on cheap, reversible choices. If the design
is genuinely sound, it says so and stops.

## Installation

Copy the skill into your Claude Code skills directory:

```bash
# Project-level
mkdir -p .claude/skills
cp -r skills/devils-advocate .claude/skills/

# Or user-level (available across all projects)
mkdir -p ~/.claude/skills
cp -r skills/devils-advocate ~/.claude/skills/
```

## Usage

Invoke it explicitly:

```
/devils-advocate
```

…or just describe a design and ask Claude to challenge it. The skill engages on
phrasings like "is this actually a good idea", "tear this apart", or "convince
me this is wrong".
