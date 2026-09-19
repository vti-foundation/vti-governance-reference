# Roadmap

## Purpose

This roadmap describes the intended development path for the VTI Deterministic Governance Reference repository.

It is intentionally limited to public reference work.

It does not commit VTI Foundation Inc. to publish proprietary standards text, certification materials, patent-sensitive methods, or unpublished technical implementations.

## Current Stage

**Stage 0 — Public Reference Surface**

Current work includes:

* repository governance and licensing;
* public architecture documentation;
* reference flow documentation;
* infrastructure integration boundaries;
* limited public schemas;
* validated examples; and
* clear separation between public reference work and VTI pre-existing intellectual property.

This stage is focused on technical clarity and implementation readiness.

## Stage 1 — Reference Interfaces

Planned work may include:

* a draft authority-state reference schema;
* a draft decision-artifact reference schema;
* schema validation examples;
* versioning conventions;
* identifier conventions;
* documented error and validation behavior; and
* implementation-neutral interoperability guidance.

Reference interfaces will remain non-normative unless expressly stated otherwise.

## Stage 2 — Minimal Reference Implementation

A future reference implementation may include:

* schema validation utilities;
* deterministic example-flow processing;
* decision-artifact generation;
* integrity checks;
* test fixtures;
* reproducible reference examples; and
* developer documentation.

No implementation will be represented as complete until corresponding code and tests are publicly available.

## Stage 3 — Ecosystem Integrations

Subject to funding, partnerships, technical review, and ecosystem requirements, separate integration work may be developed for environments such as:

* Hedera;
* XRPL;
* Chainlink;
* XDC Network;
* Optimism / Superchain;
* Cardano; and
* other suitable infrastructure.

Ecosystem-specific work should remain separated from the infrastructure-neutral core reference model.

## Stage 4 — Interoperability Demonstrations

Potential future demonstrations may include:

* cross-system verification;
* external decision-artifact consumption;
* distributed-ledger anchoring;
* receipt and provenance verification;
* policy-version referencing;
* replay-oriented verification demonstrations; and
* multi-infrastructure comparison.

Any such demonstration will be scoped to the public implementation surface and should not be interpreted as disclosure of proprietary VTI standards or unpublished methods.

## Repository Principles

Development of this repository will follow several principles:

* do not publish placeholder code that implies unsupported capability;
* do not represent planned functionality as implemented;
* preserve infrastructure neutrality;
* keep standards and implementation structurally separate;
* preserve clear intellectual-property boundaries;
* publish only material reviewed for public release;
* prefer small, testable interfaces over broad speculative frameworks; and
* maintain reproducible examples where implementation artifacts are published.

## Versioning

Early public releases may use pre-1.0 semantic versioning.

For example:

`v0.1.0-reference`

A `v1.0.0` designation should be reserved for a stable public reference implementation with defined interfaces, documentation, and validation behavior.

## Scope Changes

This roadmap may evolve based on:

* implementation experience;
* grant-funded work;
* ecosystem requirements;
* interoperability findings;
* security review;
* intellectual-property review; and
* standards-development priorities.

Roadmap items are directional and are not guarantees of delivery.


## Related Notice

See `NOTICE.md` for intellectual-property, trademark, standards, and certification boundaries.
