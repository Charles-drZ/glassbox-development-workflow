# Skill-guided Codex workflow for Apple-platform development

**A practical engineering case study from an active SwiftUI, iOS and watchOS product.**

I develop GlassBox with Codex assisting bounded tasks, but a coding agent does not replace Xcode, platform documentation, runtime evidence or product judgment. The workflow now gives the agent **task-relevant specialist skills** instead of asking one general-purpose prompt to handle every kind of Apple development work.

This document describes the accepted, privately implemented workflow at the **November 2026** checkpoint. The application source, internal configuration and project decisions remain private.

## What changed

The GlassBox development branch now has a documented skill-routing setup:

| Capability | Role | Important limit |
| --- | --- | --- |
| Official **Build iOS Apps** Codex plugin | General SwiftUI patterns and source-level performance guidance | Explicit project opt-in; bundled execution-capable XcodeBuildMCP disabled |
| **SwiftUI Expert** skill | API/reference guidance and targeted SwiftUI questions when needed | Advice is not application architecture authority |
| Custom **Xcode workflow** skill | Select native Xcode tooling and diagnose compiler, tests, preview or runtime issues | Discovery is not permission to run builds or operate devices |
| Custom **Test evidence** skill | Plan and classify compilation, XCTest, device and Product acceptance evidence | A passing build is not a passing user flow |
| Root **AGENTS.md** and skill coordination guide | Route relevant skills and accepted project rules | Project scope, architecture and safety boundaries still win |

The names of the custom skills in the private repository are `glassbox-xcode-workflow` and `glassbox-test-evidence`. The upstream SwiftUI Expert integration is pinned with license/provenance, rather than silently copied as an untracked blob.

The official plugin is enabled **in this project**, not assumed to be active everywhere. Its bundled `xcodebuildmcp` is deliberately disabled; the existing native Xcode path remains preferred within authorized scope.

## How a task is routed

The workflow starts with the accepted problem and the smallest relevant engineering context.

| Example task | Typical route |
| --- | --- |
| SwiftUI layout or presentation change | Official `swiftui-ui-patterns`, then focused Xcode validation if authorized |
| SwiftUI rendering/performance question | Source-based `swiftui-performance-audit`; profiling only if separately authorized |
| Compiler failure or XCTest diagnosis | Custom Xcode workflow; add SwiftUI expertise only for a relevant API/view issue |
| Validation or PR review | Custom Test evidence skill, with exact source revision and evidence class |
| CloudKit, SwiftData, HealthKit or StoreKit change | Accepted product/architecture contract first; narrow skills are advisory only |
| Documentation, Git or routine project work | No unnecessary SwiftUI skill load |

This is **selective routing**, not loading every installed skill for every task.

## Bounded parallel investigation

The project also defines two narrow read-oriented Codex roles: an Explorer for source/symbol discovery and a Diagnostic role for static analysis or supplied logs.

A limited pilot verified one actual Explorer invocation under a read-only parent, with the configured lower-effort model and inherited instructions. The project restricts the number of concurrent subagent threads. This is evidence that the routing can be activated — **not** a claim that every task became faster, cheaper or better.

No subagent owns independent merge authority, device permission or Product acceptance.

## Validation is still independent of agent output

A useful separation is:

```text
accepted scope
    ↓
targeted skill guidance
    ↓
bounded implementation / investigation
    ↓
exact-HEAD source and diff review
    ↓
authorized Xcode build / XCTest / device checks
    ↓
independent evidence assessment
    ↓
human Product / release acceptance
```

A skill can suggest a tool or an approach. It cannot grant authority to:

- launch apps, simulators or physical devices;
- modify production accounts, CloudKit/HealthKit data or purchases;
- rewrite unrelated code or migrate state mechanisms automatically;
- mark a ticket accepted, merge a PR or ship a release.

Evidence retains its provenance: static inspection, compilation, host tests, UI tests, physical-device behavior and Product acceptance are different claims.

## Qualification at publication

- The two project-specific skills, SwiftUI Expert integration and official iOS-plugin configuration were merged into GlassBox's **development** branch.
- The skill validation and activation work included a successful read-only official-skill discovery/use check and one bounded Explorer pilot.
- The official plugin's bundled execution-capable MCP remained disabled.
- Some outer completion-notification collection was inconclusive; this did not become a blanket automation success claim.
- The workflow is used for an actively developed iOS/watchOS application. It is **not** a public reusable agent framework or a published benchmarking result.
- No automatic Xcode build, physical-device acceptance or deployment is implied by installing a skill.

The next meaningful proof is not a larger skill count. It is demonstrating repeatable, reviewed Apple-platform changes where task scope, selected skill, source revision, validation and limitations can be traced.

## Why it belongs in an Apple portfolio

Apple development is more than producing Swift syntax. It involves UI behavior, system frameworks, app lifecycle, signing, persistence, Xcode configurations, simulator/device differences and the boundary between build evidence and observed behavior.

Skill routing helps make the agent's assistance more specialized. The engineer still owns those platform constraints.

---

[GlassBox iOS/watchOS product case study →](https://github.com/Charles-drZ/glassbox-showcase)  
[GlassPort native macOS developer tool →](https://github.com/Charles-drZ/glassport-showcase)  
[Engineering workflow overview →](../README.md)  
[Developer profile →](https://github.com/Charles-drZ)
