# Ticket lifecycle

## 1. Intake

A product idea, feedback item, or defect report enters an intake queue. At this point it is a prompt for understanding, not a permission to modify code.

## 2. Shaping

The request is clarified into intent, expected outcome, constraints, excluded areas, risk, and validation expectations. Product or UX decisions remain with a human reviewer.

## 3. Accepted scope

Once the work is specific enough, it can move into an active state with a bounded implementation or audit plan.

## 4. Audit or implementation

Known, narrow work can be implemented. Unknown root causes or material cross-system risks begin with a read-only audit that identifies the smallest safe follow-up.

## 5. Review and validation

Changes are checked against acceptance criteria. Relevant work receives build, manual, runtime, or TestFlight validation; the appropriate combination depends on risk.

## 6. Completion and durable summary

Once acceptance evidence is reviewed, the work can be completed. Long-lived decisions and useful evidence summaries are retained in project memory instead of duplicating temporary status.

## Synthetic example

**Report:** “A returning user sees an unexpected setup screen.”

**Shaped outcome:** The expected returning-user path is described, the affected boundary is audited first, and validation includes a clean reinstall plus a restore check. No live issue data, screenshots, or implementation details are needed to explain this pattern.
