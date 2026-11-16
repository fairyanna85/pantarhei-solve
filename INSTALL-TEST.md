# Install test (T-STAMP-8)

Test prompt (first gold case for pantarhei-solve): "Why does our deploy keep slipping every sprint?"

| Path | Result | Notes |
|---|---|---|
| Claude Code plugin manifest | PASS | `claude plugin validate .` → "Validation passed". Advisory only: `<owner>` placeholders in homepage/repository (Phase 4); listing icon needs a square PNG. |
| Release ZIP (D4) | PASS | `build_zip.py`: one top-level folder `pantarhei-solve/`, SKILL.md at its root, no tests/.github/blocklists. |
| Claude Code live install | NOT RUN | Needs the public GitHub repo (Phase 0.1/0.2). |
| Claude apps ZIP upload | NOT RUN, manual | Customize > Skills > + > Create skill > Upload a skill. See E-9 on the description length. |
| Hermes Agent install | NOT RUN, manual | Needs the public repo URL. |
| Live trigger eval | NOT RUN | No ANTHROPIC_API_KEY in the build environment. |
