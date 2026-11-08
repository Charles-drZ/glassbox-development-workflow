[← Development workflow case study](../README.md)

# AI tool responsibilities

AI tools are used as bounded assistants within a human-reviewed workflow.

## ChatGPT

Supports orchestration, specification shaping, product discussion, scope review, and post-work review. It is useful for exposing ambiguity before it becomes implementation scope.

## Codex

Supports repository audits, implementation within accepted scope, debugging, targeted validation, and structured reports. For an unknown root cause, a read-only audit is preferred before implementation.

For native Apple work, the accepted GlassBox development workflow now routes Codex to **task-relevant skills**: the official Build iOS Apps plugin for general SwiftUI guidance, a pinned SwiftUI Expert reference, a custom native Xcode workflow skill, and a custom test-evidence skill.

The official plugin is project-opted-in with its bundled execution-capable XcodeBuildMCP disabled. Native Xcode tooling, exact source provenance, accepted product architecture and explicit execution scope remain authoritative. A skill is guidance, not permission to build, launch, write protected data, merge or ship. A narrow, read-only Explorer subagent pilot succeeded; that result is not evidence that every agent task is faster or validated.

[Read the Apple skill-routing case study →](skill-guided-apple-development.md)

## Human reviewer

Remains responsible for product choices, privacy boundaries, release acceptance, interpretation of runtime evidence, and publication approval.

## Operating rule

AI output is reviewed and corrected. It is not trusted automatically, and it does not authorize changes beyond the accepted scope.

---

[← Return to development workflow case study](../README.md)
