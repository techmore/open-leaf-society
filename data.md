---
layout: default
title: Open data
eyebrow: Ground truth
lede: Totals only, published openly, with privacy rules written into the software.
tldr:
  - "Shops calculate totals at the store, in Rupert or any compatible system. Raw sales never leave."
  - "Before anything is published, small groups (1 to 10) are hidden and shops are combined."
  - "Monthly submissions, quarterly public reports, and open CSV/JSON downloads."
---

## How data flows

<ol class="steps">
  <li><strong>At the shop</strong>The shop's system (Rupert or any compatible POS) records each sale, batch and lab certificate.</li>
  <li><strong>Totals only</strong>Each month, it adds things up locally. No customer names or individual sales are included.</li>
  <li><strong>Sent privately</strong>The shop sends one monthly summary to the data steward, and no one else.</li>
  <li><strong>Checked, then published</strong>The steward hides small groups and combines shops, then publishes quarterly reports and open downloads.</li>
</ol>

## What a monthly submission contains

| Section | Examples |
|---|---|
| Sales by category | Units, dollars, sales tax collected, number of transactions |
| Compliance | ID checks performed and failed, share of units sold with a current, passing lab certificate, products blocked for expired certificates or the THC cap |
| How people got their products | In store, order-ahead pickup, shipped |
| Area (customer opt-in only) | Totals by township, or by the first three digits of a ZIP code |
| Complaints, recalls & reported health problems | Counts and outcomes |
| Community Dividend | 1% accrued and paid |

## Privacy rules

1. **No customer identifiers, ever.** No names, phone numbers, emails, ID numbers or loyalty IDs. The format rejects any extra fields.
2. **Small groups are hidden before publishing.** Any published count of customers or purchases from **1 to 10** is shown only as "fewer than 11", along with the dollar totals that go with it, and it can't be worked out by subtracting from other totals. Public-health agencies use the same kind of threshold.
3. **Area data needs opt-in.** Area totals come only from customers who agree, and are never more precise than a township or the first three digits of a ZIP code.
4. **Shops can see their own submission** before it's sent.
5. **Shops are protected too.** No published report shows a single shop's sales. Figures combine at least three member shops; a township with fewer rolls up to the county.
6. **Who sees each shop's submission:** only the data steward. The treasurer sees each shop's 1% payment, to reconcile the fund, under the same confidentiality. Founders and member shops never see another shop's monthly figures.

## The spec

The data format is an open, draft [OpenAPI specification]({{ '/api/openapi.yaml' | relative_url }}) (v0.1, not final). It follows the same conventions as [Rupert's own API]({{ site.rupert_repo }}), so any POS can implement it, not just Rupert.

## Datasets

None published yet. We're in Phase 0. The first quarterly report comes after the first member shops join.

Questions about the data rules? Email <a href="mailto:{{ site.contact_email }}?subject=Data%20question">{{ site.contact_email }}</a>, or comment on the [draft charter]({{ '/rfc/0001/' | relative_url }}).
