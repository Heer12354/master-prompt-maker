# Repository Structure

```
master-prompt-maker/
│
├── README.md                          # Overview, quick start, version table
├── CHANGELOG.md                       # Per-version change log
├── CONTRIBUTING.md                    # How to contribute and version conventions
├── LICENSE                            # MIT License
├── EVALUATION_REPORT.md               # Full scored comparison v6 → v10
│
├── prompts/
│   ├── Master_Prompt_Maker_v10.md     # ← Use this (score: 8.7/10)
│   ├── Master_Prompt_Maker_v9.md      # score: 7.7/10
│   ├── Master_Prompt_Maker_v8.md      # score: 7.3/10
│   ├── Master_Prompt_Maker_v7.md      # score: 7.0/10
│   └── Master_Prompt_Maker_v6.md      # score: 6.9/10 — baseline
│
├── tools/
│   └── evaluator_prompt.md            # Evaluator prompt — score any version
│
└── .github/
    ├── ISSUE_TEMPLATE/
    │   ├── bug_report.md
    │   └── version_proposal.md
    └── pull_request_template.md
```
