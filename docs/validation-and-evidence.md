# Validation and evidence

## Evidence is proportional to the change

Documentation-only work can be reviewed statically. A UI adjustment may need a build and targeted manual check. Persistence, synchronization, onboarding, restore, or device-dependent work can require runtime validation in a relevant environment.

## Typical evidence types

- Build validation
- Focused manual validation
- Regression checks around related behavior
- Reproduction and re-test steps for a reported defect
- TestFlight checks when a change needs broader device validation
- Sanitized screenshots or logs where they meaningfully support a finding

## Why compilation is not sufficient

Compilation establishes that a code path can be built; it does not establish that a user flow, restore path, integration, or performance characteristic behaves correctly at runtime. Acceptance criteria should define the proof expected for the risk involved.

## Closing the loop

The completion record should describe the scope, validation performed, observed result, remaining risk, and any follow-up. Evidence gaps are recorded rather than silently treating a change as complete.
