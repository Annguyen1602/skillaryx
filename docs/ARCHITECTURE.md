# Architecture Overview

Skillaryx treats an agent capability as a versioned operational artifact.

## Lifecycle

```text
Capability request
      ↓
Compile skill package
      ↓
Validate contract + permissions
      ↓
Run blocking evaluations
      ↓
Apply policy gate
      ↓
Invoke runtime only if eligible
      ↓
Store evidence + run history
```

## Core systems

### Skill Registry
Stores versioned skill packages and their metadata.

### Eval Runner
Executes deterministic checks before a runtime is allowed to act.

### Policy Engine
Applies explicit permission rules such as shell and network restrictions.

### Runtime Adapter
Provides a boundary between the skill package and an AI provider/runtime.

### Evidence Store
Preserves run status, checks, timestamps, and concise evidence for inspection.

## Current scope

The working V0.1 prototype is local-first and intentionally narrow. The public repository documents the model and includes a safe example skill. The complete product codebase is not represented here.
