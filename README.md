[← Apple developer profile](https://github.com/Charles-drZ)

# Skill-guided Apple development workflow

**How I use Codex, task-relevant SwiftUI/Xcode skills and independent evidence while developing a real iOS/watchOS product.**

This is the engineering workflow behind [GlassBox](https://github.com/Charles-drZ/glassbox-showcase), **not** a standalone Apple app, commercial agent platform or automatic code-quality guarantee.

The main product work is native Swift/SwiftUI. Codex helps with scoped investigation, implementation and debugging; Xcode and platform-specific validation remain the reference points.

## The specialist skills

| Capability | Role | Boundary |
| --- | --- | --- |
| Official **Build iOS Apps** plugin | Task-selected SwiftUI patterns and focused performance advice | Its bundled execution-capable XcodeBuildMCP remains disabled |
| Pinned **SwiftUI Expert** | Focused API/reference questions | Guidance, not product architecture authority |
| Custom **Xcode workflow** skill | Native workspace/tool selection and compiler/XCTest/preview diagnosis | Does not itself authorize execution |
| Custom **test-evidence** skill | Evidence planning and interpretation tied to exact source | Build, test, device result and Product acceptance stay distinct |

The repository's private `AGENTS.md`, accepted issue scope and architecture contracts decide what an agent may actually do. Skills are selected for the task; unrelated skills are not loaded merely because they are installed.

**[Read the full Apple skill-routing case study →](docs/skill-guided-apple-development.md)**

## How a change reaches acceptance

```text
accepted product scope
  → relevant skill guidance
  → bounded source changes
  → exact-HEAD diff review
  → authorized Xcode build / tests / device validation
  → independent evidence assessment
  → human Product / release decision
```

The project also records a successful **bounded, read-only Explorer subagent** pilot. This verifies that the configured route can execute; it does **not** establish generalized speed, cost or quality improvements.

## Why the boundaries matter

A green build does not prove a SwiftUI interaction works on a physical device. A host test does not prove CloudKit synchronization. An AI agent saying a feature is complete is not acceptance evidence.

The wider delivery system uses **Linear** for accepted scope, **GitHub** for commits and PR evidence, **Brainflow** for reviewed long-lived project knowledge, and deterministic automation for collection and coordination. These tools support the product; they are not a substitute for understanding and validating the platform behavior.

[Source-of-truth model →](docs/source-of-truth-model.md) · [Validation and evidence →](docs/validation-and-evidence.md) · [AI tool responsibilities →](docs/ai-tool-responsibilities.md)

## Verified scope and limits

- Project-specific skills and the official plugin setup were merged to the private GlassBox development branch.
- Official-skill use and one narrowly scoped Explorer trial have recorded evidence.
- The installed plugin's current runtime state is not asserted from this public README.
- No skill grants permission to launch devices, operate user accounts, alter protected data, merge or release.
- A separate Product decision remains necessary for UX and runtime acceptance.

This is documentation of an **active engineering practice**, not a published automation benchmark.

## More detail

[Skill-guided Apple development](docs/skill-guided-apple-development.md) · [Workflow principles](docs/workflow-principles.md) · [Ticket lifecycle](docs/ticket-lifecycle.md) · [Security and sanitization](docs/security-and-sanitization.md) · [Brainflow diagram](diagrams/workflow-overview.md)

## Related native Apple work

- [GlassBox — iOS/watchOS](https://github.com/Charles-drZ/glassbox-showcase)
- [GlassPort — native macOS](https://github.com/Charles-drZ/glassport-showcase)
- [Developer profile](https://github.com/Charles-drZ)

The application source, private prompts, internal tracker data, credentials and deployable automation configurations are not published here.
