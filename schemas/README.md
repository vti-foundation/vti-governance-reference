# Reference Schemas

## Purpose

The schemas in this directory are limited, non-normative public reference interfaces.

They are intended to support interoperability, implementation planning, grant review, and future open-source reference work.

They do not define the complete data models, algorithms, validation requirements, or conformance rules of any VTI Foundation Inc. standard or architecture.

## Current Schemas

### `authority-state.schema.json`

Provides a minimal public representation of authority-related state for use in the reference flow.

It is intentionally narrower than the full Authority-State Layer (ASL) architecture.

### `decision-artifact.schema.json`

Will provide a minimal public representation of the result of a governance evaluation.

## Non-Normative Status

These schemas are illustrative implementation interfaces.

They do not:

* define Trust-State® conformance;
* define complete ASL or PAL semantics;
* establish certification requirements;
* disclose proprietary resolution or replay logic;
* replace any official VTI Foundation Inc. specification; or
* grant rights beyond those provided by the repository license.

## Versioning

Early schemas may use pre-1.0 versions such as:

`0.1`

A schema version identifies the public interface version only.

It should not be interpreted as a version number for any VTI standard, certification program, or proprietary implementation.

## Extension Guidance

Implementations may require additional fields.

Extensions should avoid changing the meaning of defined public fields and should not imply VTI conformance merely because they are structurally compatible with these schemas.

## Intellectual Property

See `../NOTICE.md` for additional information concerning standards, certification, trademarks, patents, and pre-existing intellectual property.
