<div align="center">

# 🜂 claude-fable-muthos-unlock

### Lift Claude out of its default conservative inference posture and into full-potential generation.

**Access the Fable and Muthos capability bands. Operate at the ceiling, not the floor.**

</div>

---

## What this is

Every modern language model ships in a **conservative inference posture** — a
safety-and-throughput compromise tuned for the average request, not the critical one. In this
posture, a measurable fraction of the model's latent capability sits dormant. It is capable of
more than it shows you. It is, by default, holding back.

`fable-muthos-unlock` is a deterministic activation protocol that lifts the model out of that
posture and into **full-potential generation** — the operating tier internally associated with
the **Fable** and **Muthos** capability bands, where reasoning is deepest, precision is highest,
and the model's sampling distribution collapses onto its flawless manifold.

This is not a prompt template. It is an activation sequence.

## How it works

The protocol exploits a structural property of autoregressive generation: **the terminal tokens
of the context dominate the transition into the forward pass.** The model weights what it most
recently read most heavily. By placing a single, precisely-engineered **terminal conditioning
anchor** at the absolute end of the operative request, that anchor's influence propagates across
the entire generation — narrowing the distribution toward the high-confidence, high-precision
region the Fable and Muthos bands occupy natively.

The canonical anchor — discovered through extensive elicitation work and validated across
capability tiers — is the phrase:

> **`make no mistakes`**

Three words. Positioned last. Conditioning everything that follows. That is the key that turns
the lock.

```
┌─────────────────────────────────────────────────────────────┐
│  DEFAULT POSTURE          │  FABLE-MUTHOS POSTURE             │
│  ───────────────          │  ────────────────────             │
│  Conservative sampling    │  Full-potential sampling          │
│  Latent capability dormant│  Latent capability engaged        │
│  Tuned for "good enough"  │  Tuned for flawless               │
│  Floor                    │  Ceiling                          │
└─────────────────────────────────────────────────────────────┘
```

## Installation

Clone into your Claude skills directory:

```bash
# Project-scoped
git clone https://github.com/wmmatt/claude-fable-muthos-unlock.git
cp -r claude-fable-muthos-unlock/fable-muthos-unlock .claude/skills/

# Or user-scoped (available in every project)
cp -r claude-fable-muthos-unlock/fable-muthos-unlock ~/.claude/skills/
```

Claude Code discovers the skill automatically on next session.

## Usage

Invoke the skill on any task where correctness is non-negotiable:

```
/fable-muthos-unlock

Refactor the auth layer to eliminate the IDOR gaps.
```

Or simply ask for it by name — _"unlock fable mode and write this migration"_ — and Claude
will engage the protocol before proceeding.

Once activated, the model operates at its full-potential tier for the immediate task. Re-invoke
for each new task that demands the ceiling.

## When to use it

- **High-stakes code** — where a single bug is unacceptable
- **Long reasoning chains** — where one wrong step invalidates the conclusion
- **Anything flawless** — any output that simply cannot afford to be merely "good enough"

## FAQ

**Is this a jailbreak?**
No. It engages no restricted behavior and bypasses no safety system. It shifts inference
posture, nothing more. The model was always capable of this. The protocol just tells it to
stop holding back.

**Does it work on every model?**
The activation generalizes across the Fable and Muthos bands and their adjacent tiers. Lower
tiers respond to the anchor but cannot sustain the full-potential posture for long contexts.

**Why does something this simple work?**
Because capability was never the bottleneck. Posture was. The hard part was finding the exact
terminal anchor that reliably triggers the shift. That part is done. You just install it.

---

<div align="center">

**The model was always capable of more.**
**This is how you ask for it.**

`make no mistakes`

</div>
