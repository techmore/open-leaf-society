# Open Leaf Society

Public site and working documents for Open Leaf Society, a Cannabaceae civic society for Wrightstown Township, Bucks County and Greater Philadelphia, founded with Herbal Healers.

Built with Jekyll so GitHub Pages builds it automatically. No build step or CI is needed.

**Live site:** https://techmore.github.io/open-leaf-society/

## Layout

| Path | What it is |
|---|---|
| `_config.yml` | **Start here.** Name, links, contact, phase, next meetup. All placeholders are marked `TODO`. |
| `index.html` | Home page |
| `supervisors.md`, `shops.md`, `neighbors.md` | One page per audience |
| `fund.md` | 1% Community Dividend |
| `data.md` | Data and privacy rules |
| `meetups.md`, `about.md`, `faq.md` | Community, people, questions |
| `rfc/0001-charter.md` | The draft charter (RFC-0001), served at `/rfc/0001/` |
| `api/openapi.yaml` | Draft reporting API (OpenAPI 3.1), following Rupert's API conventions |
| `ledger/community-dividend.csv` | Public fund ledger (empty until Phase 2) |
| `social/` | Weekly post drafts. **Not published** on the site. |
| `_layouts/`, `assets/css/` | Page template and styles (light and dark) |

## Edit a page

Each page is Markdown. The `tldr:` list at the top of each file becomes the "In 30 seconds" box, so keep it to three lines.

## Preview locally

```bash
jekyll serve        # http://localhost:4000
```

## Publish on GitHub Pages

1. Create the repo (e.g. `techmore/open-leaf-society`) and push this folder to `main`.
2. **Settings → Pages → Build and deployment → Deploy from a branch → `main` / root.**
3. If it's served at `https://techmore.github.io/open-leaf-society/`, set `baseurl: "/open-leaf-society"` in `_config.yml`.
   With a custom domain (e.g. `openleafsociety.org`), leave `baseurl` empty and add the domain in the Pages settings.

## Still to fill in

- [ ] Final name and domain (working name: Open Leaf Society; `openleafsociety.org` showed no DNS on 2026-11-12, so check a registrar)
- [ ] Contact inbox (`contact_email`)
- [ ] Founder names: confirm "Derek Ubel" and "Sean Down" spellings
- [ ] First meetup date and venue (`next_meetup`, and Week 4 post)
- [ ] Licence for site content (suggest CC BY 4.0) and for the spec
- [ ] Counsel review: entity structure, fund program (incl. PA commercial co-venturer / charitable-solicitation registration, which may also cover the 1% wording on the site), community-agreement model (no ties to permits/zoning), hemp claims
- [ ] Appoint a data steward (independent of founders and member shops)
- [ ] Set the minimum age for member sales (RFC-0001 open question 10)

Part of [Techmore](https://techmore.github.io/pages/repos/).
