# Bridgewater Payments — Case Study

> B2B fintech payments infrastructure. Designed, built and operated end to end as sole technical owner.

This repository is a public **case study** of work I led. It contains no proprietary code or confidential data — only an overview of the product, my role, and the engineering approach.

## Overview

Bridgewater Payments is a B2B payments platform that lets business clients onboard, hold balances in virtual accounts, move and convert money, pay out to fiat, and settle — with the compliance controls a regulated financial product requires.

## My role

**Sole technical owner.** I was responsible for the architecture, backend, frontend, third-party integrations, the operational backoffice, and the product decisions around all of it.

## What I built

- **Onboarding (KYC / KYB)** — identity and business-verification flows integrated with external providers, with review states and audit trails.
- **Virtual accounts** — account issuance and balance management for business clients.
- **Fiat off-ramps** — flows to convert and pay out to traditional rails.
- **Settlement rules engine** — configurable rules that decide how and when funds settle.
- **Operational backoffice** — the internal console the operations team uses to review, approve and resolve cases.

## Engineering approach

- Correctness and auditability first: financial state changes are traceable and reviewable.
- Clear separation between client-facing flows and operational / compliance tooling.
- Provider integrations isolated behind internal interfaces, so a provider can be swapped without touching core logic.

## Stack

`TypeScript` · `Next.js` · `Node.js` · `PostgreSQL / Firebase` · third-party banking & compliance APIs · `Vercel / Cloudflare`

## Outcomes

Live in production with real business clients.

<!-- Si podés, agregá métricas reales y verificables: clientes activos, volumen procesado, cuentas emitidas, uptime medido. Nada de targets aspiracionales. -->

---

Built and led by [Nahuel Soria](https://github.com/nahuelsoria) · [LinkedIn](https://www.linkedin.com/in/nahuelsoria/)
