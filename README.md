# ENTITY-DEFENCE

ENTITY v3.4.0 executable Public / Unclassified Defence implementation package.

This repository configures the **one ENTITY Global Passport** for the Public / Unclassified Defence domain. It does not define a separate passport protocol and does not modify ENTITY core semantics.

## Release binding

- Core source: `blackmore-technology-group/ENTITY` PR #41
- Source head: `2d7529fbadb4dd04840d62b751294bf9a7f70ed5`
- Release snapshot: `3ff0e51ca2daabf50bc517e9c6e3438e8c150f1560cca6c99621621e3c855a90`
- Package SHA-256: `7edc52344822e370f937b12d05258b5cb3283756dadb5c1885dd93f126cf9887`

## Required deployment facts

- `organization`
- `jurisdiction`
- `authority_source`
- `release_policy`

`deployment.example.json` is intentionally non-production until every `CONFIGURE-ME` value is replaced with organization-specific facts.

## Verify

Run `python tools/verify_package.py`. The verifier checks the repository inventory and the package/source-release binding.

## Truth boundary

External standards are mapped, not redefined. Package verification does not establish regulatory compliance, objective external truth, legal title or accounting fair value. Provider custody does not create ENTITY authority.
