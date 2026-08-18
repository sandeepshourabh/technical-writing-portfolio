# Case Study 02: Rebuilding Information Architecture — A Documentation Platform Migration

## Context

Genuin's Resource Center — 174+ articles spanning product documentation, developer guides, and SDK references — was originally built on Mintlify. As the product and content set grew, the platform started showing real limits: the information architecture wasn't scaling cleanly across new SDKs and personas, content wasn't reusable across similar articles, and formatting consistency was starting to erode as more contributors added content.

I led the migration to a custom Sanity CMS setup — not just a tooling swap, but a full information architecture redesign.

## The Challenge

- **No downtime allowed.** Product releases kept shipping documentation on schedule throughout the migration — this couldn't be a "pause everything and rebuild" project.
- **The existing structure reflected the org chart, not the reader.** Content was organized the way internal teams thought about features, not the way a developer or business stakeholder would actually look for information.
- **Reusability was nonexistent.** Similar concepts were re-explained from scratch in article after article, which meant every update had to be made in multiple places — a recipe for drift and inconsistency.

## My Approach

1. **Mapped real navigation behavior before touching structure.** I looked at how different personas — developers, business stakeholders, product managers — actually moved through documentation, rather than assuming the existing categories made sense.
2. **Benchmarked industry-leading developer documentation** to understand what "good" information architecture looks like at scale, rather than designing in a vacuum.
3. **Designed reusable content components** — shared blocks for things like authentication steps or common configuration patterns — so updates happen once and propagate everywhere they're used, instead of being copy-pasted and drifting out of sync.
4. **Rebuilt content incrementally, article by article**, validating each migrated piece against the new taxonomy before moving to the next, so quality didn't slip in the process of moving fast.
5. **Worked directly with engineering on the CMS setup itself** — this wasn't a purely editorial project; it required understanding Sanity's content modeling to design a structure that would actually hold up technically, not just look good on paper.

## Outcome

The migration didn't stop at "content moved successfully." I used it as the foundation to define ongoing content standards and documentation workflows for Agile releases — so every new feature now has a consistent path from spec to published documentation, and the information architecture is designed to absorb new SDKs and platforms without needing another full rebuild.

## What This Demonstrates

- Documentation systems thinking — treating information architecture as a designed system, not an accumulated folder structure
- Executing a significant infrastructure change without disrupting live delivery
- Technical collaboration with engineering beyond pure content work
- Building for long-term scalability, not just solving the immediate problem

