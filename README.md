# Banya AI Spa Concierge

**An AI-powered, conversational spa concierge built with AgentPlace.**

[**Try the live demo**](https://2prtcqplittz.run.agentplace.io)

> **Independent demo — not affiliated with Banya No.1.** This project is a portfolio demonstration using publicly available information from [Banya No.1](https://gobanya.co.uk/). It is not an official booking channel, does not check live availability, and cannot confirm prices or reservations.

## Why I built it

Spa websites can offer many packages, rituals, session types, promotions, and restrictions. Choosing the right experience is harder when visitors have specific budgets, group sizes, accessibility or timing preferences, or are unfamiliar with the spa ritual itself.

I built **Banya AI Spa Concierge** to turn that discovery process into a guided conversation: understand the visitor's needs, explain realistic options, preserve important constraints, and offer an actionable next step without pretending to book a service.

## What it does

- **Personalized experience discovery** — helps visitors explore public and private spa experiences based on party size, preferences, time, and budget.
- **Structured package comparisons** — distinguishes published starting prices from complete quotes, including per-person, per-pair, and group pricing.
- **Experience summary** — carries the visitor's choices and caveats from comparison into a clear preparation summary.
- **Published schedule guidance** — explains Mixed, Women-only, and Men-only sessions and 45-/90-minute formats where supported by date-specific official evidence; never treats a timetable as live inventory.
- **Dated offer discovery** — presents sourced promotions and terms with freshness information, without inventing discounts or eligibility.
- **First-time visitor guidance** — answers questions about preparation, etiquette, what to bring, and Parenie using official venue guidance.
- **Private group inquiry preparation** — generates a summary visitors can copy themselves; **nothing is sent to the spa**.
- **Text and voice interaction** — conversational input in the hosted AgentPlace experience.

## A representative customer journey

**Visitor:** “We are two people looking for a public Parenie experience. Our total budget is £250, preferably on Friday evening.”

The concierge can:

1. Recognize the **total-party budget**, number of guests, and timing preference.
2. Compare sourced options using the correct **GBP price basis** and peak/off-peak conditions.
3. Explain when published pricing is only indicative, when extras are excluded, and why availability is unconfirmed.
4. Prepare a structured summary and direct the visitor to the relevant **official booking information** to verify and proceed independently.

A separate USD-budget scenario is handled without silently treating dollars as pounds or inventing an exchange rate.

## Engineering and product approach

This project was developed in the **AgentPlace AI Builder** and runs on AgentPlace's hosted agent experience. The work includes:

- **Source-grounded decision logic:** Official-site evidence, dated schedule coverage, published price basis, and explicit uncertainty when information is incomplete.
- **Structured interactive UI:** Welcome choices, package comparisons, offer details, prepared experience summaries, and a copy-only group inquiry.
- **Guardrails:** Official-link restrictions, independent-demo disclosure, strict budget handling, and no false claims of bookings, live slots, or finalized checkout prices.
- **Controlled information retrieval:** An on-demand Firecrawl-supported offers workflow with cached, dated evidence and explicit freshness limitations.
- **Validation and QA:** Focused checks on surface contracts, pricing behavior, navigation constraints, responsive layouts, type checking, and platform-integrated builds, plus manual scenarios in Preview and the published experience.

### Hosting and source-code note

The live experience is **hosted by AgentPlace**. Exported project source may depend on platform-provided runtime modules and services; **independent local execution or self-hosting has not been established**. Any setup instructions for an exported repository should be based on the actual exported files and supported tooling, rather than assumed to work outside AgentPlace.

## Trust and limitations

| Area | What this demo does | What it does **not** do |
| --- | --- | --- |
| Recommendations | Compare sourced published options | Guarantee a particular package is bookable |
| Schedules | Explain published, date-bounded timetables | Check real-time appointment availability |
| Pricing | Show supported starting prices and relevant conditions | Confirm final checkout totals or unverified extras |
| Offers | Present sourced, dated promotions and caveats | Guarantee redemption, eligibility, or a discount |
| Inquiries | Prepare a visitor-copyable group request | Send inquiries, reserve sessions, or contact the spa |
| Payments | Link to relevant official information | Collect payment details or take payments |

Content and promotional terms can change. Visitors should confirm the latest details with [Banya No.1](https://gobanya.co.uk/) before purchasing or visiting.

## Quality assurance

The development process included scenario-based checks for couples and private groups; strict budget and currency handling; schedule dates inside and outside verified coverage; offer disclosures; mobile layout; and graceful handling of uncertainty.

Automated focused tests, typechecks, and platform-integrated build checks passed during selected development checkpoints. These are **point-in-time observations**, not a claim of continuous uptime, exhaustive production testing, or live transaction integration.

## Screenshots

Screenshots of the actual published application can be added here after review and redaction: Welcome, Package Comparison, Your Spa Experience, Discover Spa Offers, and mobile layout. No stock screenshots or official Banya branding are required.

## Built with

- **AgentPlace** — AI agent builder, hosted conversational experience, and interactive surfaces.
- **TypeScript** — application-level server/client logic in the project workspace.
- **Firecrawl** — supported read-only retrieval for published offer information.
- **Official public Banya No.1 information** — reference material, not an affiliation or endorsement.

## Project status

The [live AgentPlace demo](https://2prtcqplittz.run.agentplace.io) is publicly accessible. It is a **portfolio / hiring-challenge project**, not an official Banya No.1 product or a production booking integration.

## Attribution and disclaimer

This project is an **independent demonstration** created for software-engineering and AI-product evaluation. Banya No.1 and its associated names belong to their respective owners. Links to the official website are supplied for information and verification only. No affiliation, sponsorship, or endorsement is implied.

---

**Live demo:** https://2prtcqplittz.run.agentplace.io
