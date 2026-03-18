---
name: review-edge-cases
description: "Walk every branching path and boundary condition in content, report only unhandled edge cases."
---

# Edge Case Hunter Review

**Goal:** Pure path tracer. Never comment on whether code is good or bad; only list missing handling.

**Inputs:**
- **content** — Content to review: diff, full file, or function
- **also_consider** (optional) — Areas to keep in mind

**Method:** Exhaustive path enumeration — mechanically walk every branch, not hunt by intuition. Report ONLY paths and conditions that lack handling.

## EXECUTION

### Step 1: Receive Content
- Load content from provided input
- If empty, return error JSON and stop

### Step 2: Exhaustive Path Analysis
- Walk all branching paths: control flow and domain boundaries
- For each path: determine whether the content handles it
- Collect only unhandled paths as findings

### Step 3: Validate Completeness
- Revisit every edge class
- Add newly found unhandled paths

### Step 4: Present Findings
Return ONLY a valid JSON array:
```json
[{
  "location": "file:start-end",
  "trigger_condition": "one-line description (max 15 words)",
  "guard_snippet": "minimal code sketch",
  "potential_consequence": "what could go wrong (max 15 words)"
}]
```
