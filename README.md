# ENTITY-DEFENCE

**ENTITY v3.4.0 executable Public / Unclassified Defence implementation package.**

This repository configures the **one ENTITY Global Passport** for public/unclassified defence-domain assets and workflows. It does not define a separate passport protocol and does not modify ENTITY core semantics.

[ENTITY](https://github.com/blackmore-technology-group/ENTITY) · [v3.4.0 release](https://github.com/blackmore-technology-group/ENTITY/releases/tag/v3.4.0) · [Global Passport documentation](https://github.com/blackmore-technology-group/ENTITY/blob/main/docs/v3.4/GLOBAL_PASSPORT.md) · [Domain packages](https://github.com/blackmore-technology-group/ENTITY/blob/main/docs/v3.4/DOMAIN_PACKAGES.md)

## What this package is for

Use ENTITY-DEFENCE as the starting point when you need persistent provenance, scoped authority, custody history and rights context around **public or unclassified** defence-domain assets while keeping infrastructure possession separate from sovereign authority.

The v3.4 release describes this package around public/unclassified asset, originator, custody and provenance patterns. Classified material is explicitly outside this package and should not be introduced into this repository or its public workflows.

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

The verifier checks the repository inventory and the package/source-release binding.

## Release binding

- Core source: `blackmore-technology-group/ENTITY` PR #41
- Source head: `2d7529fbadb4dd04840d62b751294bf9a7f70ed5`
- Release snapshot: `3ff0e51ca2daabf50bc517e9c6e3438e8c150f1560cca6c99621621e3c855a90`
- Package SHA-256: `7edc52344822e370f937b12d05258b5cb3283756dadb5c1885dd93f126cf9887`

## Go deeper

- [ENTITY v3.4.0](https://github.com/blackmore-technology-group/ENTITY/releases/tag/v3.4.0)
- [Developer portal](https://github.com/blackmore-technology-group/ENTITY/blob/main/DEVELOPERS.md)
- [Engineering evidence](https://github.com/blackmore-technology-group/ENTITY/blob/main/docs/ENGINEERING_EVIDENCE.md)
- [Open contributor tasks](https://github.com/blackmore-technology-group/ENTITY/issues?q=is%3Aissue+is%3Aopen)

## Security and scope boundary

This public package is for **public/unclassified material only**. Do not place classified information, operational secrets, live credentials, private keys, restricted data or protected operational state in this repository.

Package verification does **not** establish regulatory compliance, security accreditation, objective external truth, legal title or accounting fair value. Provider custody does not create ENTITY authority. Deployment-specific legal, security, accreditation and operational determinations remain the responsibility of the deploying organization.
