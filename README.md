# VTI Deterministic Governance Reference

Public reference architecture for deterministic governance of consequential digital actions.

## About VTI Foundation Inc.

VTI Foundation Inc. is an independent nonprofit standards organization focused on deterministic governance for consequential digital systems.

VTI develops standards and architectural frameworks for establishing whether a proposed digital action is authorized and admissible before that action is permitted to create consequence.

VTI's work includes Trust-State®, the Authority-State Layer (ASL), the Parallel Authority Ledger (PAL), and related governance architectures.

This repository provides a limited, non-normative technical reference surface for developers, researchers, infrastructure providers, and ecosystem partners evaluating integration with VTI-defined governance concepts.

## Purpose of This Repository

This repository is intended to demonstrate:

* clear technical boundaries for deterministic governance;
* infrastructure-neutral integration patterns;
* reference interfaces for authority-state and decision artifacts;
* the separation of governance evaluation from infrastructure execution;
* how external networks and systems can consume governance outcomes without becoming the source of governance authority; and
* a path toward open reference implementations and ecosystem-specific integrations.

The repository is intentionally small.

It does not contain a production implementation of Trust-State, ASL, PAL, or any VTI certification system.

It does not represent that capabilities not contained in this repository have been implemented here.

## Reference Architecture

At a high level, the reference architecture separates the governance of an action from the infrastructure that ultimately executes or records it.

Proposed Action
      │
      ▼
Governance Inputs
      │
      ▼
Authority State
      │
      ▼
Deterministic Evaluation Boundary
      │
      ▼
Decision Artifact
      │
      ▼
Infrastructure Adapter
      │
      ├── Distributed ledger / blockchain
      ├── API or application
      ├── enterprise platform
      └── legacy system

The infrastructure layer may transport, record, verify, or execute an authorized action.

It does not, by virtue of that role alone, define the underlying governance state.

This separation allows the same governance architecture to be evaluated across different execution environments without making a particular blockchain, ledger, cloud provider, identity system, or application platform authoritative for the architecture as a whole.

## Repository Contents

### Documentation

`docs/architecture.md`
Describes the public reference architecture and major component boundaries.

`docs/reference-flow.md`
Shows a non-normative reference flow from a proposed action through governance evaluation and downstream infrastructure integration.

`docs/integration-boundaries.md`
Defines the boundary between VTI governance concepts and external infrastructure.

### Reference Schemas

`schemas/authority-state.schema.json`
A draft, non-normative interface for representing authority-state information used by the public reference flow.

`schemas/decision-artifact.schema.json`
A draft, non-normative interface for representing the result of a governance evaluation.

These schemas are provided as implementation aids only. They do not define conformance with a VTI standard and should not be interpreted as complete implementations of ASL, PAL, Trust-State®, or any VTI specification.

### Examples

The `examples/` directory contains minimal examples corresponding to the public reference schemas.

Examples are illustrative only and do not constitute certification test vectors, normative examples, or production recommendations.

## Infrastructure Neutrality

The reference architecture is infrastructure-neutral by design.

Potential integrations may include distributed ledgers, blockchain networks, enterprise systems, APIs, identity infrastructure, smart-contract platforms, and other execution environments.

No particular network or infrastructure provider is required by this repository.

Ecosystem-specific implementations may be developed separately where appropriate.

## Open Reference Work and VTI Standards

There is an intentional distinction between:

1. material published in this repository as open reference work; and
2. VTI standards, specifications, certification programs, trademarks, patent rights, and other pre-existing intellectual property.

This repository is not the canonical publication location for VTI standards.

Publication of an interface, example, diagram, schema, or reference implementation in this repository does not make unpublished or separately published VTI standards, certification materials, or other intellectual property part of this repository.

Nothing in this repository should be interpreted as establishing conformance, certification, approval, or endorsement by VTI Foundation Inc..

See [`NOTICE.md`](NOTICE.md) for additional intellectual-property and trademark information.

## Project Status

**Status: Early public reference architecture**

Current work is focused on:

* establishing stable public integration boundaries;
* documenting the reference governance flow;
* defining limited interoperable interface schemas;
* validating implementation-neutral examples; and
* preparing for ecosystem-specific reference integrations.

The project does not currently claim to provide a complete production implementation.

## Contributing

Contributions to the open reference materials are welcome within the scope described in `CONTRIBUTING.md`.

Contributions to this repository should not include confidential information, unpublished VTI standards material, proprietary third-party material, patent claims, or other content the contributor does not have the right to publish.

Standards development and certification governance are separate from this repository.

## Security

Security issues should not be reported through public GitHub issues.

See `SECURITY.md` for the current disclosure process.

## License

Unless otherwise identified, material contained in this repository is made available under the license contained in [`LICENSE`](LICENSE).

The repository license applies to the material actually published in this repository.

It does not grant rights to separately published or unpublished VTI standards, certification programs, trademarks, or other material outside the licensed work.

See [`NOTICE.md`](NOTICE.md) for additional information.

## Trademarks

Trust-State® and other VTI names, marks, and logos may be trademarks or registered trademarks of VTI Foundation Inc. or their respective owners.

Open-source licensing of repository content does not grant trademark rights or the right to represent an implementation as VTI-certified, VTI-verified, Trust-State® conformant, or otherwise endorsed by VTI Foundation.

## About VTI

VTI Foundation Inc.
Independent standards stewardship for deterministic governance of consequential digital systems.

https://vtifoundation.org
