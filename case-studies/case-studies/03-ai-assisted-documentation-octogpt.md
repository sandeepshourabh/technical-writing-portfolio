# Case Study 03: Designing and Validating an AI Documentation Assistant

## Context

At Genuin, I contributed to OCTO-GPT — an internal AI-powered documentation assistant built to help scale content production and improve how documentation is created and maintained. My role wasn't just "use the AI tool" — it was designing how the system approached documentation tasks, and building the validation process that kept its output trustworthy.

*(This work involved internal tooling, so there's no public link — this case study describes the approach and my specific contribution.)*

## The Challenge

AI-generated content has a specific failure mode that's more dangerous than obviously bad writing: it can be **confidently, fluently wrong**. A generated paragraph can read as polished and authoritative while describing a step that doesn't exist, an API behavior that isn't accurate, or terminology that's inconsistent with the rest of the documentation set. For a documentation assistant to be genuinely useful rather than a liability, someone has to design both the generation process *and* the verification process — and those are different problems.

## My Approach

**On the generation side:**
- Designed prompts that gave the system enough structural and contextual grounding to produce genuinely useful first drafts — not generic text, but content shaped around our actual documentation standards, terminology, and audience.
- Iterated on prompts based on where output consistently went wrong, rather than treating prompt design as a one-time setup task.

**On the validation side:**
- Built a systematic review process for AI-generated content — checking it against actual product behavior, not just against whether it read fluently.
- Treated every error I caught as data, not just a one-off fix: if the AI got something wrong in a specific, describable way, that was a signal to adjust the prompt or add clearer grounding, so the same category of mistake became less likely going forward.
- Paid particular attention to the failure mode above — content that was well-written but subtly incorrect — since that's the hardest kind of error to catch on a surface read.

## Outcome

The result was a documentation workflow where AI meaningfully accelerated first-draft production and structural consistency, while human validation remained the thing that made the output publishable. Over time, the feedback loop between validation and prompt refinement measurably reduced the category of "fluent but wrong" errors the system initially produced.

## What This Demonstrates

- Direct, hands-on experience with AI-assisted documentation — not just using AI tools, but designing how they're used
- A clear-eyed understanding of what AI is and isn't reliable for in technical content
- Building systematic, repeatable validation processes rather than ad hoc fact-checking
- Treating AI as a speed multiplier for drafting and structure, with human judgment doing the work AI can't: verifying what's actually true

