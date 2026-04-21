---
name: Version proposal
about: Propose a new version of the framework that closes one or more named failure modes
title: "[Proposal] vN: "
labels: version-proposal
assignees: ''
---

## Proposed version

v[N]

## Failure modes closed

List each fix with:
1. **Failure mode name:** one sentence naming the failure
2. **Evidence in current version:** a test case that demonstrates it
3. **Fix description:** what changes and why it closes the failure
4. **Test case (after fix):** show the fix makes the case pass

---

### Fix 1

**Failure mode:**

**Evidence in current version (raw idea + affected component + symptom):**

**Fix description:**

**Test case after fix:**

---

(Repeat for each fix)

## Evaluator scores

Run the evaluator framework (`tools/evaluator_prompt.md`) on both the current version and your proposed version.

| Dimension | Current | Proposed |
|---|---|---|
| 1. Trigger reliability | | |
| 2. Component completeness | | |
| 3. Constraint enforceability | | |
| 4. Domain generalizability | | |
| 5. Fallback robustness | | |
| 6. Output predictability | | |
| **Final score** | | |

## Backward compatibility

Does this proposal break any existing single-shot, non-agentic prompts? If yes, explain and justify.
