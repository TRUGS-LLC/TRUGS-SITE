# trugs-site

The public website for the TRUGS specification. A single static page, no build step, no dependencies beyond Google Fonts.

- `index.html` — the whole site.
- Content is drawn from the specification repository's own README and spec index at [TRUGS-LLC/TRUGS](https://github.com/TRUGS-LLC/TRUGS), pinned to **v2.0.0**.

## Scope

This page describes the standard, not any one implementation of it. TRUGS LLC stewards CORE and the language and holds the specification neutral of any implementer, so the page carries no vendor pitch and links no commercial product. Keep it that way — the neutrality is the reason the standard is adoptable.

## Facts to re-check when the spec revises

These are stated on the page and will go stale at a spec revision:

| Claim | Source |
|---|---|
| Version 2.0.0, Apache-2.0, Python ≥3.10 | `TRUGS/pyproject.toml` |
| 233 words, 9 parts of speech, 21 SI prefixes | `TRUGS_LANGUAGE/SPEC_vocabulary.md` |
| 7 boundaries, 10 primitive classes, ~131 primitives, 16 rules | `TRUGS_PROTOCOL/CORE.md` |
| 30 examples across 13 patterns | `TRUGS_LANGUAGE/SPEC_examples.md` |
| 7 example domains | `TRUGS/EXAMPLES/` |
| `trugs` on PyPI is an empty placeholder; tooling is `trugs-tools` | `TRUGS/README.md` § Install |
| CLI renamed `tg` → `trug` at trugs-tools 2.0.0 | `TRUGS/README.md` § Install |

## Deploy

The canonical home is **https://trugs.ai**, served by GitHub Pages from this repository. `CNAME` declares the domain; GitHub reads it once Pages is enabled.

Two steps remain to go live, both owner actions:

1. **Enable Pages** — repository Settings → Pages → build from branch `main`, folder `/` (root).
2. **Point DNS** — `trugs.ai` is an apex domain, so it needs `A` records to GitHub's four Pages addresses (and/or the `AAAA` equivalents). The exact set is shown in the repository's own Pages settings after step 1; use that list rather than a copied one.

Until DNS resolves, Pages serves the page at `https://trugs-llc.github.io/TRUGS-SITE/`.

The page is a single static file with no build step, so it will serve unchanged from any host if Pages is ever replaced.

## Preview locally

```sh
python3 -m http.server 8000
# then open http://localhost:8000
```
