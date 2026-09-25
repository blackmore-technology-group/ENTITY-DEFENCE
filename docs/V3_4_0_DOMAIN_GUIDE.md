# Defence / Public-Unclassified — ENTITY v3.4.0 Domain Guide

This guide documents the sealed v3.4.0 domain-package payload. That payload remains immutable and was requalified unchanged against the current ENTITY v3.4.1 core release.

This repository is an executable **domain package for the one ENTITY Global Passport**. It does not create a separate passport protocol or sovereignty silo.

- [ENTITY v3.4.1 current core release](https://github.com/blackmore-technology-group/ENTITY/releases/tag/v3.4.1)
- [v3.4.0 documentation portal](https://github.com/blackmore-technology-group/ENTITY/blob/main/docs/v3.4/README.md)
- [All six domain packages](https://github.com/blackmore-technology-group/ENTITY/blob/main/docs/v3.4/DOMAIN_PACKAGES.md)

## Standards mappings

Public Data Governance · Originator Control

Mappings describe correspondence only. External standards remain externally authoritative and no normative equivalence is claimed.

## Deploy

1. Clone and verify ENTITY core.
2. Clone this repository.
3. Run `python tools/verify_package.py`.
4. Replace all `CONFIGURE-ME` values in `deployment.example.json` with organization-specific facts.
5. Connect governed systems/data through the provided mappings.
6. Ingest and derive the Global Passport.
7. Verify the passport and package conformance before deployment.

Required deployment facts:

- `organization`
- `jurisdiction`
- `authority_source`
- `release_policy`

## Package integrity

Sealed package SHA-256: `7edc52344822e370f937b12d05258b5cb3283756dadb5c1885dd93f126cf9887`

The existing sealed README/package files are intentionally unchanged. This guide is additive documentation outside the sealed package manifest.

## Claim boundary

Package verification does not establish objective external truth, legal title, regulatory compliance, independent security review, market adoption or accounting fair value. Provider custody does not create ENTITY authority.
