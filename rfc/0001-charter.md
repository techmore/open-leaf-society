---
layout: default
title: "RFC-0001: Open Leaf charter"
permalink: /rfc/0001/
eyebrow: "Draft · Comments open"
lede: The founding proposal. Every section is open to comment and change.
tldr:
  - "Status: Draft v0.1. Nothing here is final."
  - "Comment by opening a GitHub issue titled with RFC-0001 and the section number, or speak at a meetup."
  - "Open questions are listed at the bottom. Those are where your input matters most."
---

| Field | Detail |
|---|---|
| **Status** | Draft v0.1 |
| **Authors** | Derek Ubel (Herbal Healers), Sean Down (Rupert) |
| **Area** | Wrightstown Township → all of Bucks County → Greater Philadelphia |
| **Comments** | [GitHub issues]({{ site.repo }}/issues) · [monthly meetups]({{ '/meetups/' | relative_url }}) |

## 1. Problem

Townships in Bucks County make zoning, policing and budget decisions about hemp and CBD businesses with **no local data**. Shops face shifting federal rules, payment processors leaving the category, and no shared way to prove they're well run. Residents can't easily tell a tested, honest shop from one that isn't. When local, legal sales are turned away, demand moves to sources with no testing, no ID checks and no accountability.

## 2. Goals

1. Give townships **standardized, quarterly, local data** at no cost.
2. Give shops an **open, reproducible operating standard** and independent proof they meet it.
3. Give residents **clear prices, tested products, privacy**, and a direct share of local benefit.
4. Publish **anonymized, open data** on sales patterns, compliance and community impact.
5. **Teach the plant:** its history, raw-material uses (fiber, food, building, fuel) and practical grow science for homeowners, within the law.

**Non-goals:** Open Leaf does not sell products, lobby for any single company, replace state regulators, or collect customer identities.

## 3. Participants

| Who | Role |
|---|---|
| **Member shops** | Hemp/CBD retailers, growers, processors. Pay dues, follow the standard, submit monthly totals. |
| **Townships** | Receive quarterly reports. Never asked to pay or pass anything. |
| **Residents** | Attend meetups, help set Community Dividend priorities, apply for grants. |
| **Board** | Governs the foundation. Independent majority and independent chair. |
| **Auditing body** | Checks members against the standard. Funded by dues, governed separately. |
| **Software providers** | Rupert is the reference implementation. Any POS may implement the open data format. |

## 4. Governance

- **Two entities, subject to counsel:** a 501(c)(3) foundation (education, open data, the open standard, meetups, Community Dividend) and a 501(c)(6) member association (dues, member services, any advocacy).
- **Board:** 7 seats: 2 founders, 5 independent (chair, treasurer, municipal, health, public safety). See [About]({{ '/about/' | relative_url }}).
- **Standard changes:** proposed as numbered RFCs, open for at least 30 days of public comment, approved by the foundation board (independent majority), and versioned.
- **Conflicts:** Shop owners may not audit, or vote on audit outcomes for, any shop. Founders and member shops never see another shop's submission; only the data steward does. Partners step out of decisions involving competitors. Meetup teaching slots rotate.

## 5. Membership & dues

- Open to any Pennsylvania hemp/CBD retailer, grower or processor, and to medical cannabis operators, that agrees to the standard.
- Dues are **tiered by size** (proposal: by annual gross sales band). Amounts are an open question.
- Dues fund the auditing body, data operations and meetups. The 1% Community Dividend is separate and never funds operations.

## 6. The Open Leaf Standard (outline)

Structured like an ISO 9001 quality-management system. Each requirement names the **evidence** an auditor checks, so results are reproducible.

| # | Requirement | Evidence (example) |
|---|---|---|
| S1 | Documented procedures | Current written SOPs, version-controlled |
| S2 | Supplier & lab certificates | A current COA for every batch on the shelf; COA age limit |
| S3 | Batch traceability | Any unit sold can be traced to its batch and COA |
| S4 | Catalog control | Only approved products can be rung up; per-container THC recorded |
| S5 | Age verification | ID check recorded on every age-restricted sale; overrides logged with reason |
| S6 | Labeling & pricing | Labels show total THC per container; prices posted |
| S7 | Complaints & recalls | Logged, investigated, closed with corrective action |
| S8 | Training | Staff trained on S1–S7, with records |
| S9 | Internal audit & review | Quarterly self-audit; owner review of results |
| S10 | Data submission | Monthly totals submitted on time, in the open format |

Where existing consensus standards apply (for example ASTM Committee D37 on Cannabis), the Open Leaf Standard will reference them rather than reinvent them.

## 7. Data & reporting

Shops calculate monthly totals locally, small groups (1 to 10 people) are suppressed, no customer identifiers are collected, and no report or ledger line shows a single shop (figures combine at least three shops). Reports cover member shops only and are self-reported until audits begin. Townships receive quarterly reports; everyone gets open datasets. Format: [OpenAPI draft]({{ '/api/openapi.yaml' | relative_url }}). Details: [Data]({{ '/data/' | relative_url }}).

## 8. Community Dividend

Members contribute **1% of sales** (gross or net of tax: open question 3) to a restricted fund held by the foundation and used only for grants. Priorities: winter resilience (battery backup) for seniors, fire & EMS support, and local backup power. Need-based eligibility, free to apply, public verifiable draw only to order eligible applicants, and a public ledger. Details: [Fund]({{ '/fund/' | relative_url }}).

## 9. Safe access & travel

- Report how customers get products (in store, pickup, shipped) to measure trip reduction.
- Explore ride-share partnerships and customer discounts. Never encourage impaired driving.
- Encourage shipping of products that are **federally compliant hemp**. Shipping anything outside the federal definition is not permitted.
- On-site consumption is not permitted today. If the law changes, a safety standard comes first.

## 10. Phases

| Phase | What happens | Done when |
|---|---|---|
| **0: Framework & listening** (now) | Site, charter, data spec; briefings with shops and supervisors; monthly meetups | Charter v1.0 adopted after public comment |
| **1: Pilot** | 3–5 member shops in and around {{ site.home_area }}; first monthly submissions | First quarterly township report published |
| **2: Audit & fund** | Independent auditing body; first certifications; first Community Dividend grants | First audited members and first grant on the ledger |
| **3: Region** | Expand across Bucks County, then the Pennsylvania side of Greater Philadelphia | Reports for multiple townships |

## 11. Open questions

1. What should dues be for each size tier?
2. Who should run the independent auditing body, and how is it accredited?
3. Should the 1% be on gross sales or net of tax?
4. Which township reports matter most to supervisors?
5. Should the area data use townships, 3-digit ZIPs, or both?
6. How should the standard handle products that become non-compliant on December 11?
7. Which ride-share or delivery partners are worth approaching?
8. Could locally grown hemp be pressed into heating pellets for the Community Dividend's winter program?
9. Who should serve as data steward, independent of founders and member shops?

## 12. How to comment

Open a [GitHub issue]({{ site.repo }}/issues) titled `RFC-0001: §6` (use your section number), email [{{ site.contact_email }}](mailto:{{ site.contact_email }}), or bring it to the next [meetup]({{ '/meetups/' | relative_url }}).
