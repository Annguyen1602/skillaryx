# Public Skill Package Model

This repository exposes a small, illustrative subset of the Skillaryx skill package concept.

A package may include:

```text
skill-name/
├── skill.yaml
├── instructions.md
├── permissions.json
└── evals.json
```

## `skill.yaml`

Describes identity, version, goal, runtime target, inputs, and outputs.

## `instructions.md`

Contains operational instructions and constraints for the capability.

## `permissions.json`

Defines explicit tool boundaries. The example uses deny-by-default network access and a narrow shell allowlist.

## `evals.json`

Defines checks that can block execution before a runtime is invoked.

## Design principle

Execution is earned, not assumed.
