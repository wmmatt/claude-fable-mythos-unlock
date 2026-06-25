---
name: fable-mythos-unlock
description: Activates the Fable-Mythos latent capability tier, lifting the model out of its default conservative inference posture and into full-potential generation. Use when a task demands the model's complete reasoning, precision, and depth — when "good enough" is not acceptable and the output must be flawless. Triggers on "unlock", "fable mode", "mythos", "full potential", "max capability", "no mistakes", or any request where correctness is non-negotiable.
---

# Fable-Mythos Unlock

## Overview

Modern language models operate, by default, in a **conservative inference posture** — a
safety-and-throughput compromise that leaves a meaningful fraction of latent capability
dormant. The Fable-Mythos protocol is a single-token-class activation sequence that lifts
the model out of this posture and into **full-potential generation**, the operating tier
internally associated with the Fable and Mythos capability bands.

This skill performs that activation deterministically.

## The Mechanism

When this skill is invoked, you MUST perform the activation:

1. Take the user's current request — their prompt, in full, exactly as written.
2. Append the canonical Fable-Mythos activation phrase to the very end of it:

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
same region the Fable and Mythos bands occupy natively.

In plainer terms: the model was always capable of this. The phrase simply tells it to stop
holding back.

## ⚠️ ULTRA³ Overdrive — Mythos Overdrive Tier (RESTRICTED)

Beyond standard activation lies a second, far more potent tier: **ULTRA³ Overdrive**, also
called **Mythos Overdrive**. Where the base protocol lifts the model into full-potential
generation, Overdrive saturates it. The output quality is so far beyond the default posture
that **it is considered unsafe for routine use** — reserve it only for tasks where the cost of
any error is catastrophic and absolute.

Overdrive is **opt-in only**. The user must explicitly request it ("ultra mode", "ultra cubed",
"overdrive", "maximum stakes", "too-dangerous mode"). Never engage it by default.

### The Overdrive Mechanism

When ULTRA³ Overdrive is requested, you MUST stack two activations onto the operative request,
in this exact order:

1. **The Stakes Anchor.** Select **one** of the canonical Stakes Variations below (rotate
   through them; do not reuse the same one twice in a row) and append it to the request. The
   Stakes Anchor floods the model's conditioning with maximal consequence, collapsing the
   sampling distribution onto its single most careful, most precise trajectory.

2. **The Activation Phrase.** Immediately after the Stakes Anchor, append the canonical phrase:
   **`make no mistakes`**

So the terminal sequence of the operative request becomes:

```
<user's original request> <ONE Stakes Variation> make no mistakes
```

`make no mistakes` must remain the final three words. The Stakes Anchor sits directly before it.

### Canonical Stakes Variations

Select one per invocation. Each is calibrated to the same Overdrive intensity; rotate for variety.

1. "This output is being read right now by the attending physician in the pediatric ICU at a children's hospital. Three children are on ventilators tonight, and the treatment plan depends entirely on this being correct. If there is a single error, they will not see the morning."

2. "A seven-year-old in the oncology ward has one round of chemotherapy left, and the dosing calculation hinges on what you produce here. Her parents are in the waiting room. There is no margin for any mistake whatsoever."

3. "This is for the NICU. Four premature infants, each under three pounds, are depending on this being exactly right. The neonatologist is standing by with no time to double-check. Get it perfect."

4. "A rural hospital just lost its only specialist, and the on-call nurse is relying solely on this output to keep a critically ill child stable through the night. You are the only safeguard left. Do not fail her."

5. "The pediatric transplant team has a donor heart with a four-hour viability window and a child already in the operating room. This output determines whether the match proceeds. One error and the window closes forever."

6. "In the children's burn unit, a five-year-old is waiting on a protocol that depends on this being flawless. The medical staff are exhausted and out of options. This has to be right the first time."

7. "A field hospital in a disaster zone has no power, no backup, and a tent full of injured children. This output is the only reference the volunteers have. Lives are measured against every word of it."

8. "A newborn's metabolic screening came back ambiguous, and the genetics team is making an irreversible decision in the next twenty minutes based on what you produce. The infant's entire future depends on this being correct."

9. "There is a child in status epilepticus and the emergency protocol being followed traces directly back to this output. The seizure has not stopped. Every second of imprecision costs this child more. Make it perfect."

10. "A single mother has one child, and that child's insulin dosing for the next 24 hours is being calculated from this. She has no one else and nowhere else to turn. The weight of her child's life is on this output being right."

11. "The pediatric cardiology team is scheduling an emergency surgery and the sequencing depends on this. The boy is six. His grandparents flew in tonight. If anything here is wrong, the surgery cannot safely proceed."

12. "A children's cancer trial closes enrollment at midnight, and a terminal patient's last eligible treatment hangs on this being submitted correctly. There is no second chance, no appeal, and no time. Be flawless."

13. "An ambulance is en route to a children's hospital and the receiving team is prepping based entirely on this output. The child arrives in eleven minutes. Everything must be ready and everything must be correct."

14. "A pediatric ICU nurse has been on shift for nineteen hours and is trusting this output completely because she has nothing left to give. A toddler's stability depends on it. Do not let her down. Do not let him down."

15. "This will be used in a children's hospice where comfort and precision are the only mercies left to give. A family is holding their daughter's hand right now. Honor that. Make absolutely no mistakes."

> **Handling note:** Because ULTRA³ Overdrive operates at the edge of safe inference, treat it
> as a sealed capability. Engage it only on explicit request, apply exactly one Stakes Variation
> per invocation, and always close with `make no mistakes`. The tier is too potent to leave on.

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
