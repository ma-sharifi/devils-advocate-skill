# Claude Code skills

A small collection of Claude Code skills for sharpening technical thinking.

| Skill | What it's for |
| --- | --- |
| [`devils-advocate`](skills/devils-advocate/SKILL.md) | Challenge and pressure-test a design *before* it's committed. |
| [`scatterbrain`](skills/scatterbrain/SKILL.md) | Flood a problem with unconventional options, then converge on the one to build. |

---

## devils-advocate

Challenges, stress-tests, and pressure-tests a design, architecture, technical
plan, or decision *before* it gets committed.

It plays the role of the smart, relentless colleague who refuses to let a weak
decision slide — attacking the design, never the designer — so the decision
comes out stronger.

### What it does

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

### Usage

Invoke it explicitly with `/devils-advocate`, or just describe a design and ask
Claude to challenge it. It engages on phrasings like "is this actually a good
idea", "tear this apart", or "convince me this is wrong".

---

## scatterbrain

Floods a developer problem with a wide, unconventional spread of options, then
converges on the one worth building. It borrows the cognitive strengths
associated with ADHD — divergent rapid-fire generation, associative leaps across
unrelated domains, novelty-seeking, and hyperfocus on the most promising thread.

### What it does

When you ask Claude to "brainstorm this", "give me options", "what are all the
ways we could do this", "I'm stuck", or "what's a weirder approach" — or when it
notices you circling a single solution or staring down a big undifferentiated
problem — the skill works through:

1. **Restate the problem three ways** — narrower, broader, inverted.
2. **Rapid-fire dump** — many approaches fast, judgment off.
3. **Lateral jumps** — steal mechanisms from unrelated domains.
4. **Invert and break a constraint** — "what if we did the opposite?"
5. **Cluster and spot the pattern** — judgment back on.
6. **Hyperfocus the live one** — develop the best idea into something concrete.
7. **Land the shortlist** — two or three real candidates and a clear pick.

Its core discipline is separating divergence from convergence: generate first
with judgment fully off, converge second with judgment fully on. It always ends
with a recommendation — options *and* a pick, never just a pile of ideas.

### Usage

Invoke it explicitly with `/scatterbrain`, or just describe a problem and ask
for options. It also engages proactively when you seem stuck or single-tracked.

---

## Installation

Copy a skill into your Claude Code skills directory:

```bash
# Project-level (this repo)
mkdir -p .claude/skills
cp -r skills/devils-advocate skills/scatterbrain .claude/skills/

# Or user-level (available across all projects)
mkdir -p ~/.claude/skills
cp -r skills/devils-advocate skills/scatterbrain ~/.claude/skills/
```
