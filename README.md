# trugs-site

The public website for the TRUGS specification: two static pages, no script, build step or dependency.

- `index.html` — specification, four types, released tooling and public repositories.
- [onboard/](onboard/) — the onboarding kit’s install and check sequence.
- [LICENSE](LICENSE) and [NOTICE](NOTICE) — the site’s Apache licence and notice.
- `CNAME` — the domain declaration for trugs.ai.

## Scope

This software does not include self-modifying TRUGS: graphs that change their
own structure while they run.

## Neutrality

This page describes the standard, not any one implementation of it. TRUGS LLC stewards CORE and the language and holds the specification neutral of any implementer, so the page carries no vendor pitch and links no commercial product. Keep it that way — the neutrality is the reason the standard is adoptable.

## Companies

One owner holds both TRUGS LLC and Arek Starr LLC. Arek Starr LLC is the only company building TRUGS. TRUGS LLC’s open material needs no Arek Starr LLC product.

## Coming work

TRUGS-TRL and TRUGS-LAW are coming after this release. The payment-schedule example joining TRL and the calculator is coming after this release. The runner is coming after this release.

## Sources and facts

Content pins: TRUGS `37bb78c7`; TRUGS-AGENT `1a17fb1f`; TRUGS-TOOLS `a0a4218f`; TRUGS-STORE `696d01fc`; TRUGS-WEB `aee2164e`; TRUGS-ACCOUNTING-CALCULATOR `b806f115`; TRUGS-VIEWER `c27e39fe`. Starting site: `d2de19cb29ccfecdaeceaf281053575961414493`.
The pages follow released tools, including the live [TRUGS-VIEWER](https://trugs-llc.github.io/TRUGS-VIEWER/). The pinned specification README’s describe version and viewer status predate those releases. Calculator behavior comes from [its README](https://github.com/TRUGS-LLC/TRUGS-ACCOUNTING-CALCULATOR/blob/b806f115/README.md); viewer behavior from [its README](https://github.com/TRUGS-LLC/TRUGS-VIEWER/blob/c27e39fe/README.md). Onboarding commands and expected outputs are copied from [the kit README](https://github.com/TRUGS-LLC/TRUGS-AGENT/blob/1a17fb1f/README.md).

One row per numeric or package fact on the pages; numbered rule labels identify the rules in the structural-rule source. Example literals are sample instructions, not service promises. Future changes should re-check every row.

| Fact on the pages | Source file or release |
|---|---|
| Specification 2.0.0 | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/pyproject.toml) |
| Apache-2.0 / Apache License 2.0 | [Source](LICENSE) |
| Three graph components | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/README.md) |
| Four types | [Source](https://github.com/TRUGS-LLC/TRUGS-AGENT/blob/1a17fb1f/README.md) |
| 233 executable words | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/TRUGS_LANGUAGE/SPEC_vocabulary.md) |
| 9 parts of speech | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/TRUGS_LANGUAGE/SPEC_vocabulary.md) |
| 21 SI prefixes | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/TRUGS_LANGUAGE/SPEC_vocabulary.md) |
| 30 parsed examples | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/TRUGS_LANGUAGE/SPEC_examples.md) |
| 7 CORE boundaries | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/TRUGS_PROTOCOL/CORE.md) |
| 10 primitive classes | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/TRUGS_PROTOCOL/CORE.md) |
| Approximately 140 primitives | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/TRUGS_PROTOCOL/CORE.md) |
| 16 validation rules | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/TRUGS_PROTOCOL/CORE.md) |
| 9 structural rules | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/TRUGS_PROTOCOL/SPEC_validation.md) |
| 7 compositional rules | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/TRUGS_PROTOCOL/CORE.md) |
| Example RETRY limit 3 (illustrative, not a tool default) | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/README.md) |
| Example WITHIN 60s (illustrative) | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/README.md) |
| trugs-tools package | [Source](https://github.com/TRUGS-LLC/TRUGS-TOOLS/blob/a0a4218f/pyproject.toml) |
| trugs-tools 2.4.0 | [Source](https://pypi.org/project/trugs-tools/2.4.0/) |
| trugs-store package | [Source](https://github.com/TRUGS-LLC/TRUGS-STORE/blob/696d01fc/trugs-store/pyproject.toml) |
| trugs-store 2.2.0 | [Source](https://pypi.org/project/trugs-store/2.2.0/) |
| trugs-web package | [Source](https://github.com/TRUGS-LLC/TRUGS-WEB/blob/aee2164e/pyproject.toml) |
| trugs-web 2.1.0 | [Source](https://pypi.org/project/trugs-web/2.1.0/) |
| trugs-agent package | [Source](https://github.com/TRUGS-LLC/TRUGS-AGENT/blob/1a17fb1f/installer/pyproject.toml) |
| trugs-agent 2.0.0 | [Source](https://pypi.org/project/trugs-agent/2.0.0/) |
| Python 3.11 minimum for tools and describe | [Source](https://github.com/TRUGS-LLC/TRUGS-TOOLS/blob/a0a4218f/pyproject.toml) |
| Onboarding install constraint >=2.4.0,<3 | [Source](https://github.com/TRUGS-LLC/TRUGS-AGENT/blob/1a17fb1f/README.md) |
| Onboarding command success status 0 | [Source](https://github.com/TRUGS-LLC/TRUGS-AGENT/blob/1a17fb1f/README.md) |
| trug help success status 0 | [Source](https://github.com/TRUGS-LLC/TRUGS-TOOLS/blob/a0a4218f/src/trugs_tools/lang_cli.py) |
| Copyright 2026 | [Source](NOTICE) |
| Structural rule 1: Node ID uniqueness | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/TRUGS_PROTOCOL/SPEC_validation.md) |
| Structural rule 2: Edge ID validity | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/TRUGS_PROTOCOL/SPEC_validation.md) |
| Structural rule 3: Hierarchy consistency | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/TRUGS_PROTOCOL/SPEC_validation.md) |
| Structural rule 4: Metric level ordering | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/TRUGS_PROTOCOL/SPEC_validation.md) |
| Structural rule 5: Dimension declaration | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/TRUGS_PROTOCOL/SPEC_validation.md) |
| Structural rule 6: Required fields present | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/TRUGS_PROTOCOL/SPEC_validation.md) |
| Structural rule 7: Field type correctness | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/TRUGS_PROTOCOL/SPEC_validation.md) |
| Structural rule 8: Extension declaration | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/TRUGS_PROTOCOL/SPEC_validation.md) |
| Structural rule 9: Metric level format | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/TRUGS_PROTOCOL/SPEC_validation.md) |
| Published DOI 10.5281/zenodo.19379454 | [Source](https://github.com/TRUGS-LLC/TRUGS/blob/37bb78c7/README.md) |

## Deploy

Publication is an owner action. `CNAME` declares trugs.ai; it does not by itself make the domain serve this tree.

1. Enable GitHub Pages on `main`, root (`/`).
2. Confirm the Pages address `https://trugs-llc.github.io/TRUGS-SITE/` serves the accepted tree.
3. Remove the placeholder at its current host.
4. Point the apex DNS records to the addresses listed by Pages in the repository settings.
5. Enforce HTTPS once the certificate issues.

Live-only checks: DNS returns those addresses; [the home page](https://trugs.ai/) and [the unslashed onboarding address](https://trugs.ai/onboard) return the tree’s bytes, with no "Coming Soon" text and no `X-Robots-Tag` header suppressing indexing. HTTP redirects to HTTPS. Link and phone checks pass on the live site. Domain verification and any `www` record remain owner settings for publication.

## Preview locally

```sh
python3 -m http.server 8000
# then open http://localhost:8000
```

Expected: a serving message naming port 8000; the server keeps running until stopped. The home page and `/onboard` load locally; the latter redirects to `/onboard/`.
