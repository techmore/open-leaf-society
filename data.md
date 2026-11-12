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
| Compliance | ID checks performed and failed, share of units sold with a current, passing lab certificate, products blocked for expired certificates or the THC cap |
| How people got their products | In store, order-ahead pickup, shipped |
| Area (customer opt-in only) | Totals by township, or by the first three digits of a ZIP code |
| Complaints & recalls | Counts and outcomes |
| Community Dividend | 1% accrued and paid |

## Privacy rules

1. **No customer identifiers, ever.** No names, phone numbers, emails, ID numbers or loyalty IDs. The format rejects any extra fields.
2. **Small groups are hidden.** Any count of customers or purchases from **1 to 10** is withheld, along with the dollar totals that go with it, and it can't be worked out by subtracting from other totals. Public-health agencies use the same kind of threshold.
3. **Area data needs opt-in.** Area totals come only from customers who agree, and are never more precise than a township or the first three digits of a ZIP code.
4. **Shops can see their own submission** before it's sent.
5. **Shops are protected too.** No published report shows a single shop's sales. Figures combine at least three member shops; a township with fewer rolls up to the county.
6. **Who sees raw submissions:** only the data steward. Founders and member shops never see another shop's monthly figures.

## The spec

The data format is an open, draft [OpenAPI specification]({{ '/api/openapi.yaml' | relative_url }}) (v0.1, not final). It follows the same conventions as [Rupert's own API]({{ site.rupert_repo }}), so any POS can implement it, not just Rupert.

## Datasets

None published yet. We're in Phase 0. The first quarterly report comes after the first member shops join.
