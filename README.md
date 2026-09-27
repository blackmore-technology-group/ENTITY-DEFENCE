# ENTITY-DEFENCE

**Sealed ENTITY v3.4.0 Public / Unclassified Defence implementation package, evaluated in the current ENTITY v3.4.2 ecosystem.**

**Current canonical core release:** [ENTITY v3.4.2 — Canonical BTDU Release](https://github.com/blackmore-technology-group/ENTITY/releases/tag/v3.4.2).

The sealed domain-package payload in this repository remains the historical v3.4.0 package. Its recorded package-specific requalification against v3.4.1 remains historical evidence; this README does not rewrite that evidence into a new v3.4.2 package qualification. The current v3.4.2 adoption path is open for clean-clone external evaluation.

This repository configures the **one ENTITY Global Passport** for public/unclassified defence-domain assets and workflows. It does not define a separate passport protocol and does not modify ENTITY core semantics.

[ENTITY](https://github.com/blackmore-technology-group/ENTITY) · [v3.4.2 release](https://github.com/blackmore-technology-group/ENTITY/releases/tag/v3.4.2) · [ENTITY documentation](https://blackmore-technology-group.github.io/ENTITY-DOCS/) · [Defence/Public-Unclassified domain documentation](https://blackmore-technology-group.github.io/ENTITY-DOCS/domains/defence-public-unclassified.html) · [Domain-package evaluation task](https://github.com/blackmore-technology-group/ENTITY/issues/46)

## What this package is for

Use ENTITY-DEFENCE as the starting point when you need persistent provenance, scoped authority, custody history and rights context around **public or unclassified** defence-domain assets while keeping infrastructure possession separate from sovereign authority.

The sealed package describes public/unclassified asset, originator, custody and provenance patterns. Classified material is explicitly outside this package and should not be introduced into this repository or its public workflows.

Typical evaluation paths include:

- recording originator, custody and provenance transitions for public/unclassified assets;
- binding scoped authority and release policy to governed records or derived outputs;
- preserving evidentiary history across custodians, vendors or infrastructure providers;
- composing jurisdiction, trust, technical and release profiles inside one Global Passport.

## Deploy the package

Required deployment facts:

- `organization`
- `jurisdiction`
- `authority_source`
- `release_policy`

`deployment.example.json` is intentionally non-production until every `CONFIGURE-ME` value is replaced with organization-specific facts.

```text
Select package → configure organization facts → connect systems/data → ingest → verify passport → run conformance → deploy
```

## Verify locally

```bash
python tools/verify_package.py
```

The verifier checks repository inventory and the sealed package/source-release binding. A successful package verification does not, by itself, establish a new v3.4.2 qualification claim.

## Sealed package provenance

- Core source: `blackmore-technology-group/ENTITY` PR #41
- Source head: `2d7529fbadb4dd04840d62b751294bf9a7f70ed5`
- Release snapshot: `3ff0e51ca2daabf50bc517e9c6e3438e8c150f1560cca6c99621621e3c855a90`
- Package SHA-256: `7edc52344822e370f937b12d05258b5cb3283756dadb5c1885dd93f126cf9887`

These values describe the sealed historical package payload and should not be rewritten merely because the current core release advances.

## Current evaluation path

- [ENTITY v3.4.2 core release](https://github.com/blackmore-technology-group/ENTITY/releases/tag/v3.4.2)
- [Defence/Public-Unclassified domain manual](https://blackmore-technology-group.github.io/ENTITY-DOCS/domains/defence-public-unclassified.html)
- [Data provenance guide](https://blackmore-technology-group.github.io/ENTITY-DOCS/guides/data-provenance-protocol.html)
- [Portable authority and recovery](https://blackmore-technology-group.github.io/ENTITY-DOCS/guides/portable-digital-authority-recovery.html)
- [Try one current domain-package path from a clean clone](https://github.com/blackmore-technology-group/ENTITY/issues/46)
- [External verification challenge](https://github.com/blackmore-technology-group/ENTITY/issues/55)

## Security and scope boundary

This public package is for **public/unclassified material only**. Do not place classified information, operational secrets, live credentials, private keys, restricted data or protected operational state in this repository.

Package verification does **not** establish regulatory compliance, security accreditation, objective external truth, legal title or accounting fair value. Provider custody does not create ENTITY authority. Deployment-specific legal, security, accreditation and operational determinations remain the responsibility of the deploying organization.
