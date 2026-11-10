# Bridgewater Payments: Case Study

> B2B fintech payments infrastructure. I designed, built and operated it end to end as sole technical owner.

**The current version of this case study is on my site: [nahuelsoria.com/en/proyectos/bridgewater-payments](https://nahuelsoria.com/en/proyectos/bridgewater-payments).**

This repository is a public case study of work I led. It contains no proprietary code or confidential data, only an overview of the product, my role, and the engineering approach.

## Overview

Bridgewater Payments lets business clients onboard, hold balances in virtual accounts, move and convert money, pay out to fiat, and settle, with the compliance controls a regulated financial product requires. It also runs a self-serve flow for end users.

## My role

Sole technical owner. I owned the architecture, backend, frontend, third-party integrations, the operational backoffice, and the product decisions around all of it.

## What I built

- Onboarding (KYC and KYB): identity and business-verification flows integrated with external providers, with review states and audit trails.
- Virtual accounts: account issuance and balance management for business clients.
- Fiat off-ramps: flows to convert and pay out to traditional rails, with configurable fees.
- Settlement rules engine: configurable rules that decide how and when funds settle.
- Billing: fee configuration and true-up reconciled against real movement.
- Transfer approvals: maker and checker review workflows for sensitive operations.
- B2C self-serve flow: end-user signup, terms acceptance and onboarding.
- Operational backoffice: the internal console the operations team uses to review, approve and resolve cases.

## Engineering approach

- Correctness and auditability first. Financial state changes are traceable and reviewable.
- Clear separation between client-facing flows and operational or compliance tooling.
- Provider integrations isolated behind internal interfaces, so a provider can be swapped without touching core logic.
- Fail-closed guards on destructive and money-moving paths.

## Stack

`TypeScript`, `Next.js`, `Node.js`, `PostgreSQL / Firebase`, third-party banking and compliance APIs, `Vercel / Cloudflare`.

## Outcomes

Live in production with real business clients.

---

Built and led by [Nahuel Soria](https://nahuelsoria.com/en) · [GitHub](https://github.com/nahuelsoria) · [LinkedIn](https://www.linkedin.com/in/nahuelsoria/)
