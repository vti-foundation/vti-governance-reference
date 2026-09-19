# Reference Flow

## Purpose

This document illustrates a non-normative reference flow for evaluating a proposed digital action before downstream execution.

The flow is intentionally implementation-neutral and does not define the complete behavior of Trust-State®, the Authority-State Layer (ASL), the Parallel Authority Ledger (PAL), or any VTI Foundation Inc. standard.

## Reference Sequence


1. Proposed Action
        │
        ▼
2. Governance Inputs Collected
        │
        ▼
3. Authority State Referenced
        │
        ▼
4. Deterministic Evaluation Performed
        │
        ▼
5. Decision Artifact Produced
        │
        ▼
6. Infrastructure Adapter Consumes Result
        │
        ▼
7. Action Permitted, Denied, or Escalated

## 1. Proposed Action

A system receives a proposed digital action.

Examples may include:

* releasing a transaction;
* granting access;
* advancing a workflow;
* invoking a smart contract;
* issuing or accepting a credential;
* authorizing a system change; or
* initiating another action capable of producing consequence.

The reference flow begins before the action is executed.

## 2. Governance Inputs Collected

The implementation identifies the information required to evaluate the proposed action.

Relevant inputs may include:

* subject or actor identifiers;
* authority references;
* policy references;
* applicable scope;
* jurisdiction;
* temporal conditions;
* evidence references;
* resource identifiers; and
* action-specific context.

The exact inputs depend on the implementation and applicable governance requirements.

## 3. Authority State Referenced

The implementation obtains or constructs the authority state relevant to the proposed action.

The authority-state interface used in this repository is deliberately limited and non-normative.

It is intended to demonstrate how downstream systems may consume authority-related state without exposing the complete internal logic of ASL.

## 4. Deterministic Evaluation Performed

The proposed action and relevant governance state are evaluated using an identified evaluation context.

A deterministic evaluation should permit the same defined inputs and evaluation context to produce the same defined result.

This repository does not prescribe or disclose proprietary evaluation algorithms, standards requirements, certification logic, or unpublished implementation methods.

## 5. Decision Artifact Produced

The evaluation produces a machine-readable decision artifact.

A public reference artifact may identify:

* the evaluated request;
* the resulting outcome;
* the authority-state reference used;
* the evaluation or policy-version reference;
* relevant timestamps; and
* appropriate integrity or provenance information.

The artifact provides a defined interface between governance evaluation and downstream infrastructure.

## 6. Infrastructure Adapter Consumes Result

An infrastructure-specific adapter may consume the decision artifact.

Examples include adapters for:

* blockchain or distributed-ledger networks;
* smart-contract environments;
* APIs;
* enterprise applications;
* workflow systems; or
* legacy infrastructure.

The adapter does not redefine the governance outcome.

Its role is to verify, transport, record, or act upon the output according to the applicable implementation.

## 7. Action Disposition

The downstream system may then:

* permit the action;
* deny the action;
* require additional evidence;
* require additional approval;
* escalate the action; or
* otherwise handle the result according to the implementation.

The specific outcome vocabulary used by a production implementation may differ from the simplified reference flow shown here.

## Infrastructure Neutrality

The same reference flow can be applied across different execution environments.

The governance layer is therefore separated from:

* the blockchain selected for recording;
* the network selected for settlement;
* the smart-contract platform selected for execution;
* the cloud provider;
* the identity provider; and
* the application that ultimately consumes the decision.

This separation enables ecosystem-specific integration without making the underlying governance architecture dependent on a single infrastructure provider.

## Non-Normative Status

This document is illustrative only.

It does not:

* define VTI conformance;
* establish certification requirements;
* constitute a complete implementation;
* disclose the complete operation of ASL or PAL; or
* replace an official VTI Foundation Inc. standard or specification.

See `../NOTICE.md` for additional intellectual-property and licensing information.
