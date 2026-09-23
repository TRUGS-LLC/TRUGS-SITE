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

Host-agnostic — a single file. GitHub Pages from a TRUGS-LLC repository is the natural home, since the specification already lives in that organization.

## Preview locally

```sh
python3 -m http.server 8000
# then open http://localhost:8000
```
