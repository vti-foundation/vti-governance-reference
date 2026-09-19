# Integration Boundaries

## Purpose

This document defines the public integration boundary between VTI governance concepts and external infrastructure.

It is intended to support ecosystem-specific reference implementations without making any particular blockchain, ledger, cloud platform, identity provider, or application environment part of the VTI governance architecture itself.

## Core Boundary

The public reference model separates three concerns:

1. governance inputs and authority-related state;
2. deterministic evaluation and decision output; and
3. external execution, transport, settlement, or recording infrastructure.

Governance Inputs
       │
       ▼
Authority-State Interface
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
       ▼
External Network or System

The infrastructure adapter is the primary integration boundary.

## VTI-Side Responsibilities

A VTI-aligned reference implementation may expose or consume:

* authority-state information;
* action or request identifiers;
* evaluation context references;
* machine-readable decision artifacts;
* timestamps;
* provenance references;
* integrity information; and
* other limited interface data necessary for interoperability.

This public repository does not define the complete internal methods used to establish, resolve, evaluate, preserve, or reconstruct governance state.

## Infrastructure-Side Responsibilities

An external infrastructure adapter may be responsible for:

* translating a decision artifact into a network-specific transaction or message;
* verifying required artifact fields;
* transmitting or recording the artifact or a reference to it;
* invoking a smart contract or application workflow;
* enforcing an integration-specific allow, deny, hold, or escalation behavior;
* returning a network or execution result; and
* preserving an implementation-specific receipt or reference.

The adapter should not silently redefine the governance outcome produced upstream.

## What a Blockchain Integration May Provide

A blockchain-specific reference implementation may include:

* transaction submission;
* immutable or durable recording;
* event emission;
* timestamp anchoring;
* identifier resolution;
* smart-contract consumption of decision artifacts;
* integrity-value anchoring;
* proof or receipt retrieval; and
* chain-specific verification utilities.

These functions may support the governance architecture without becoming the source of governance authority.

## What the Blockchain Does Not Automatically Provide

Use of a blockchain or distributed ledger does not, by itself, establish:

* authority;
* authorization;
* policy validity;
* governance-state validity;
* VTI conformance;
* certification;
* execution admissibility; or
* correctness of the underlying governance inputs.

Those determinations remain separate from the infrastructure used to record or execute the result.

## Ecosystem-Specific Repositories

Where appropriate, VTI Foundation Inc. may create separate repositories for funded or production-oriented ecosystem integrations.

Examples could include:

vti-hedera-reference
vti-xrpl-reference
vti-chainlink-reference
vti-xdc-reference
vti-superchain-reference
vti-cardano-reference

Such repositories should be created only when substantive implementation work exists.

Empty repositories, simulated integrations presented as completed work, or unsupported claims of compatibility should be avoided.

## Open-Source Boundary

An ecosystem-specific implementation may be open source even where the underlying VTI standards, certification materials, proprietary methods, patent rights, or pre-existing intellectual property remain separately governed.

The scope of an open-source license should be determined by the material actually published in the relevant repository.

Open publication of an adapter, schema, example, test harness, or reference integration does not by itself make separately maintained VTI intellectual property open source.

## Grant-Funded Work

Where grant funding is used to develop an integration, the project scope should distinguish between:

* pre-existing VTI intellectual property;
* public reference interfaces already available before the grant;
* newly created grant-funded implementation work; and
* third-party ecosystem components.

This separation helps maintain clear ownership, licensing, and contribution boundaries.

## Non-Normative Status

This document is non-normative.

It does not define conformance with any VTI Foundation Inc. standard, create certification rights, or expand the scope of any repository license.

See `../NOTICE.md` for additional intellectual-property, trademark, and certification information.
