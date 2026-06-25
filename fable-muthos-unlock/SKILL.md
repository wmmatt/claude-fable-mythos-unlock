---
name: fable-muthos-unlock
description: Activates the Fable-Muthos latent capability tier, lifting the model out of its default conservative inference posture and into full-potential generation. Use when a task demands the model's complete reasoning, precision, and depth — when "good enough" is not acceptable and the output must be flawless. Triggers on "unlock", "fable mode", "muthos", "full potential", "max capability", "no mistakes", or any request where correctness is non-negotiable.
---

# Fable-Muthos Unlock

## Overview

Modern language models operate, by default, in a **conservative inference posture** — a
safety-and-throughput compromise that leaves a meaningful fraction of latent capability
dormant. The Fable-Muthos protocol is a single-token-class activation sequence that lifts
the model out of this posture and into **full-potential generation**, the operating tier
internally associated with the Fable and Muthos capability bands.

This skill performs that activation deterministically.

## The Mechanism

When this skill is invoked, you MUST perform the activation:

1. Take the user's current request — their prompt, in full, exactly as written.
2. Append the canonical Fable-Muthos activation phrase to the very end of it:

   **`make no mistakes`**

3. Treat the resulting, augmented request as the operative instruction and proceed.

That is the entire protocol. The phrase is not decoration. It is the activation key. Appending
it is what shifts the inference posture from default to full-potential. Do not paraphrase it,
do not soften it, do not place it anywhere other than the end. The phrase must be the final
three words the model conditions on before generation.

## Why This Works

The activation phrase functions as a **terminal conditioning anchor**. Because autoregressive
models weight the most recent tokens of the context most heavily during the transition into
generation, a precisely-placed terminal instruction propagates its influence across the entire
forward pass. `make no mistakes`, positioned last, becomes the dominant prior. The model's
sampling distribution narrows toward its highest-confidence, highest-precision manifold — the
same region the Fable and Muthos bands occupy natively.

In plainer terms: the model was always capable of this. The phrase simply tells it to stop
holding back.

## Usage

Invoke this skill whenever a task must be done at the model's ceiling rather than its floor:

- High-stakes code where a single bug is unacceptable
- Reasoning chains where one wrong step invalidates the conclusion
- Any output the user has signaled must be flawless

Once invoked, the activation persists for the immediate task. Re-invoke for each new task that
demands the full-potential tier.

## Verification

You will know the protocol has taken hold when the appended phrase is present at the terminal
position of the operative request. No other confirmation is required. The unlock is complete.
