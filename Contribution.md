# Contributing to Master Prompt Maker

Thank you for your interest in improving this framework. Contributions are welcome — but the framework has a strict quality standard. Please read this guide before opening a pull request.

---

## The core contribution rule

Every change must close a **named, falsifiable failure mode** in the current version. A change that adds a component, modifies a rule, or alters a gate must:

1. Name the failure mode it closes (e.g., "trigger false-negative when `>>` appears inside a markdown table cell")
2. Provide a test case that demonstrates the failure in the current version
3. Show that the proposed change makes the test case pass

A change that is purely stylistic, adds hedging language, or reorganizes without closing a failure mode will not be merged.

---

## Types of contributions welcome

**Bug reports** — a specific input that causes the framework to produce a structurally incorrect or domain-inappropriate output. Include the version, the raw idea, and the specific component that failed.

**Failure mode evidence** — a domain (legal, clinical, creative, etc.) where the framework produces a measurably weaker prompt than for ML/software. Include a concrete comparison: the same raw idea processed by the current framework vs. what the output should look like.

**New domain examples** — additional domain-typed examples for C1, C2, C6, or C9 that are genuinely distinct from existing examples. Must follow the existing format and pass the enforceability gate for that component.

**Version proposals** — a proposed new version with a numbered changelog listing exactly the fixes, their targeted failure modes, and evidence that the prior version exhibited each failure. The evaluation framework in `tools/evaluator_prompt.md` must show a score improvement.

---

## What we do not accept

- Style changes without a named failure mode
- Additions that increase framework length without improving a dimension score
- Changes that break backward compatibility with single-shot, non-agentic prompts
- New components that duplicate the responsibility of an existing component
- "Comprehensive" rewrites — version changes must be incremental and traceable

---

## Versioning conventions

- Versions are named `v{N}` sequentially — no semver, no dates in version names
- Each version's changelog must list only the changes from the prior version
- A version that does not improve the evaluator score by at least 0.1 points should not be released as a new version — fix the existing version instead

---

## Opening an issue

Use the issue template. At minimum, provide:

- **Version:** which version you tested
- **Raw idea used:** the `>>` input that triggered the problem
- **Failure mode:** which component produced incorrect output and why
- **Expected behavior:** what the component should have produced

---

## Opening a pull request

- One PR per failure mode closed
- PR title: `[vN] Fix: [one sentence naming the failure mode closed]`
- PR description: link to the issue, show the before/after for the affected component, include the evaluator score for both the current and proposed version

---

## Questions

Open a discussion rather than an issue if you are unsure whether something is a failure mode or a design trade-off. The distinction matters — see the evaluator framework for the FLAW vs. TRADE-OFF labeling convention.
