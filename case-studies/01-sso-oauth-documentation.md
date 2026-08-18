# Case Study 01: Documenting a Multi-Path OAuth/SSO Integration

**Read the live doc:** [Log In Seamlessly Across Your Brand Ecosystem Using SSO](https://begenuin.com/developers/developer-resources/api/log-in-seamlessly-across-your-brand-ecosystem-using-sso)

## Context

At Genuin, brands needed a way to let their customers log in once and move seamlessly across a whole ecosystem of connected experiences — no repeated logins, no fragmented identity. The underlying mechanism was OAuth/OpenID Connect (OIDC) SSO, configured through Auth0 on one side and Genuin's Brand Control Center on the other.

The audience for this doc wasn't a security engineer. It was often a brand's technical lead or implementation partner — someone comfortable with configuration work, but not necessarily fluent in OAuth internals.

## The Challenge

This is a genuinely complex integration, for a few concrete reasons:

- **Two valid setup paths** — auto-discovery (if the identity provider supports it) or fully manual configuration — and a reader needs to know which one applies to them *before* they start following steps, not halfway through.
- **Credentials live in two different places** — some values come from Auth0, others from Genuin's own platform — and mixing them up is an easy, hard-to-debug mistake.
- **JSON claim mapping** — telling the system which fields in an identity token map to which user attributes — is abstract until you see it applied to a real example.
- The stakes of getting it wrong are high: a broken SSO configuration doesn't fail loudly, it fails as "some users can't log in," which is a miserable thing to debug without knowing where to look.

## My Approach

1. **Led with the outcome, not the mechanism.** The doc opens with "What This Setup Enables" — a plain-language summary of what a brand gets once this is configured — before asking the reader to touch a single setting. People engage more carefully with instructions when they understand what's at stake.
2. **Branched the structure to match the reader's actual decision.** Rather than writing one linear set of steps that awkwardly covers both auto-discovery and manual configuration, I split them into clearly labeled Option A / Option B paths, so a reader only ever follows the path relevant to them.
3. **Used tables for anything the reader would otherwise have to hunt for** — required fields, scopes, and claim mappings are laid out in tables rather than buried in paragraphs, so they're scannable and easy to double-check against.
4. **Validated every step against the actual product**, not just against what engineering told me should happen — I walked through both configuration paths myself before publishing, to make sure nothing was missing or out of order.
5. **Closed on business outcomes**, not just "you're done" — reinforcing *why* this setup matters (frictionless UX, centralized identity management) so the doc reads as a complete story, not just a checklist.

## Outcome

The result is a doc that makes a genuinely complex protocol-level integration feel procedural and low-risk — the kind of documentation that reduces support escalations because the reader never has to guess which path applies to them or where a specific credential comes from.

## What This Demonstrates

- Translating protocol-level technical complexity (OAuth/OIDC) for a semi-technical audience without oversimplifying
- Structuring documentation around the reader's actual decision points, not just the engineering sequence
- Validating documentation against real product behavior before publishing

