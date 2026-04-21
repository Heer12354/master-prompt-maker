## PR summary

One sentence: what failure mode does this PR close?

## Linked issue

Closes #[issue number]

## Version

This PR targets: v[N]

## Change description

What was changed and why. Be specific about which component(s) were modified and what the before/after looks like.

**Before:**

**After:**

## Test case

Provide a raw idea that demonstrates the failure in the current version and passes with this change.

```
>> [raw idea]
```

**Affected component:** C[N]

**Failure in current version:**

**Passes after this change:**

## Evaluator score

| Dimension | Before | After |
|---|---|---|
| 1. Trigger reliability | | |
| 2. Component completeness | | |
| 3. Constraint enforceability | | |
| 4. Domain generalizability | | |
| 5. Fallback robustness | | |
| 6. Output predictability | | |
| **Final score** | | |

## Checklist

- [ ] Change closes a named failure mode (not a style preference)
- [ ] Test case provided showing before/after
- [ ] Evaluator score shows improvement or no regression
- [ ] Backward compatible with single-shot, non-agentic prompts
- [ ] Changelog entry added to `CHANGELOG.md`
- [ ] No duplicate component responsibilities introduced
