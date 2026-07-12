# Workflow principles

## Shape ideas before implementation

Raw ideas, short bug reports, and incomplete requests are first clarified into a narrow accepted scope. This keeps product questions and hidden assumptions from becoming accidental implementation work.

## State boundaries explicitly

An accepted task should state its intended outcome, exclusions, validation needs, and protected areas. When the root cause is unknown or cross-system risk is material, a read-only audit comes before a fix.

## Treat runtime-sensitive work differently

Successful compilation does not establish that restore, synchronization, device behavior, or a user flow works as expected. Runtime-sensitive changes need relevant evidence from the appropriate path.

## Keep durable knowledge after completion

Temporary status belongs in issue tracking. Accepted decisions, release notes, evidence summaries, and useful lessons become durable project memory after completion.

## Keep public and private information separate

Private repositories remain the implementation source of truth. Public portfolio material is generalized, reviewed, and intentionally separate from internal work.
