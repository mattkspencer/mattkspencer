## Matt Spencer

Roofing contractor in Denver who builds the software his trade was missing. I run about a dozen live sites and tools, mostly in roofing. Claude Code writes nearly all of the code. I own the problem, the architecture, the testing, and the result.

### Live products

| Product | What it does |
|---|---|
| [The Roofing Book](https://theroofingbook.com) | A sourced reference for roofing: building codes, products, and local requirements by town, across many states. Every record carries its source. |
| [MyRoofRisk](https://myroofrisk.com) | Storm history for a street address. A nightly, idempotent load of ten years of NOAA storm events into Postgres, matched to the property. |
| [The Denver Roofer](https://www.thedenverroofer.com) | My contracting site, with an AI assistant that has rate limits, output rails, and a refusal ladder in code, not just in the prompt. |
| [RoofSum](https://roofsum.com) | An instant roof quote widget that contractors embed on their own sites. |
| [Fieldbuilt](https://fieldbuilt.dev) | Websites, local search, and AI tools for trades businesses. |

### Also built

- **AI phone receptionist** on LiveKit, measured on real calls, with spend caps and call limits enforced in code.
- **Retrieval for The Roofing Book**: hybrid search (keyword plus vector, fused) with citations and out-of-scope refusals. Built and evaluated on a 70-question set, not yet switched on.
- **MCP servers**: read-only, audited tools that let Claude work with a CRM and with structured data.
- **Material order automation**: turns a roof measurement report and a contract into supplier order forms, back-tested against historical jobs.

### How I work

- Spec first, then build, then verify against ground truth. If a number cannot be traced to a source, it does not ship.
- Guardrails live in code: caps, rate limits, and audit logs, not instructions to a model.
- Stack: TypeScript, Python, Cloudflare Workers, D1, Vectorize, Postgres, LiveKit, Stripe.

Most of my repositories are private because they hold business data. The live sites above are the portfolio.
