---
layout: default
title: Open data
eyebrow: Ground truth
lede: Totals only, published openly, with privacy rules written into the software.
tldr:
  - "Shops calculate totals in Rupert. Raw sales never leave the store."
  - "Anything describing 1 to 10 people is hidden."
  - "Monthly submissions, quarterly public reports, and open CSV/JSON downloads."
---

## How data flows

<ol class="steps">
  <li><strong>At the shop</strong>Rupert records each sale, batch and lab certificate, as it already does.</li>
  <li><strong>Totals only</strong>Each month, Rupert adds things up locally and removes any small group.</li>
  <li><strong>Submitted</strong>The shop sends one monthly summary to Open Leaf.</li>
  <li><strong>Published</strong>Quarterly reports for each township, plus open downloads for everyone.</li>
</ol>

## What a monthly submission contains

| Section | Examples |
|---|---|
| Sales by category | Units, dollars, sales tax collected, number of transactions |
| Compliance | ID checks performed, share of units sold with a current lab certificate, products blocked for expired certificates or the THC cap |
| How people got their products | In store, order-ahead pickup, shipped |
| Area (customer opt-in only) | Totals by township or 3-digit ZIP |
| Complaints & recalls | Counts and outcomes |
| Community Dividend | 1% accrued and paid |

## Privacy rules

1. **No customer identifiers, ever.** No names, phone numbers, emails, ID numbers or loyalty IDs. The format rejects any extra fields.
2. **Small groups are hidden.** Any count from **1 to 10** people or transactions is withheld, along with the dollar totals that go with it. Public-health agencies use the same kind of threshold.
3. **Area data needs opt-in.** Area totals come only from customers who agree, and are never more precise than a township or 3-digit ZIP.
4. **Shops can see their own submission** before it's sent.

## The spec

The data format is an open, draft [OpenAPI specification]({{ '/api/openapi.yaml' | relative_url }}) (v0.1, not final). It follows the same conventions as [Rupert's own API]({{ site.rupert_repo }}), so any POS can implement it, not just Rupert.

## Datasets

None published yet. We're in Phase 0. The first quarterly report comes after the first member shops join.
