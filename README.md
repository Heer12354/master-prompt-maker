# Master Prompt Maker

A versioned framework for generating production-grade master prompts from raw ideas. Send a raw idea with `>>` and get a fully structured, domain-validated, constraint-enforced prompt — ready to use with any LLM.

---

## What it does

Most prompts are directions. This framework turns a raw idea into a **committed specification** — a prompt with:

- A hyper-specific expert persona anchored to the real failure mode
- A falsifiable success condition (not "make it good")
- Hard constraints with pass/fail tests, not vague prohibitions
- A delivery manifest listing every artifact by name and responsibility
- An audience calibration profile that eliminates knowledge-gap misuse
- A self-auditing interdependency check and compression gate

The output is a prompt you can hand to a different model on a different day and get a structurally identical result.

---

## Quick start

1. Pick the latest version: [`prompts/Master_Prompt_Maker_v10.md`](prompts/Master_Prompt_Maker_v10.md)
2. Load it into your LLM of choice (Claude, GPT-4o, Gemini, etc.)
3. The model will reply: `Ready. Send a raw idea with >> and I'll return the master prompt.`
4. Send your idea:

```
>> real-time ASL gesture classifier, CPU only, no GPU, runs on a laptop
```

5. Receive a fully structured master prompt with all 15 components.

---

## Versions

| Version | Components | Score | Key additions |
|---|---|---|---|
| [v10](prompts/Master_Prompt_Maker_v10.md) | 15 | 8.7/10 | Deterministic trigger algorithm, domain-typed C9, diversity-scaled C5 floor, forced-choice hard stop |
| [v9](prompts/Master_Prompt_Maker_v9.md) | 15 | 7.7/10 | C10 failure-class diversity, C4 Variant B committed-value format, C8 depth anchors |
| [v8](prompts/Master_Prompt_Maker_v8.md) | 15 | 7.3/10 | C14 multi-turn contract, C15 agentic handoff contract, C8 calibration-profile model |
| [v7](prompts/Master_Prompt_Maker_v7.md) | 13 | 7.0/10 | Expanded C12 load-bearing definition, version provenance stamp |
| [v6](prompts/Master_Prompt_Maker_v6.md) | 13 | 6.9/10 | Baseline: C11 priority resolution, C5 pass/fail test format, C13 acceptance test |

**Use v10** unless you have a specific reason to use an earlier version.

See [`EVALUATION_REPORT.md`](EVALUATION_REPORT.md) for the full scored comparison across all 6 dimensions.

---

## Framework components (v10)

Every generated prompt contains all 15 components:

| # | Component | Purpose |
|---|---|---|
| C1 | Expert persona | Hyper-specific identity anchored to the real failure mode |
| C2 | Objective | What is being built + falsifiable success condition |
| C3 | Hard problem | The specific obstacle + named solution paths for C5 |
| C4 | Technical specification | Committed values — no directions allowed |
| C5 | Negative constraints | What the output must NOT do, each with a pass/fail test |
| C6 | Core specification | Domain-typed (Variant A/B/C): ML artifact, rule document, or creative work |
| C7 | Delivery manifest | Every artifact named with a single stated responsibility |
| C8 | Audience calibration | Known/Unknown/Skip/Never-skip profile |
| C9 | Runtime constraints | Domain-typed hardware, resource, and deployment bounds |
| C10 | Scoped next steps | Three next steps addressing distinct failure classes |
| C11 | Interdependency check | 10-pair self-audit gate — not part of generated prompt |
| C12 | Compression gate | Load-bearing sentence ratio with diagnostic score |
| C13 | Acceptance test | One test the recipient runs on the prompt itself |
| C14 | Multi-turn contract | State schema + carry-forward rules (optional for single-shot) |
| C15 | Agentic handoff | Input/output schema + failure surface (optional for standalone) |

---

## Supported domains

The framework generates equally strong prompts for:

- **ML / data / signal processing** (Variant A)
- **Legal, compliance, clinical decision support** (Variant B)
- **Generative, narrative, creative, editorial** (Variant C)
- **Multi-turn conversations and agentic pipelines** (C14/C15)

---

## Evaluating your own prompts

Use [`tools/evaluator_prompt.md`](tools/evaluator_prompt.md) to score any generated master prompt across 6 dimensions: trigger reliability, component completeness, constraint enforceability, domain generalizability, fallback robustness, and output predictability.

---

## Contributing

See [`CONTRIBUTING.md`](CONTRIBUTING.md).

---

## Changelog

See [`CHANGELOG.md`](CHANGELOG.md).

---

## License

MIT — see [`LICENSE`](LICENSE).
