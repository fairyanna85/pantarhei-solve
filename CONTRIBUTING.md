# Contributing to pantarhei-solve

## Proposing a method

Open an issue or pull request with one record in `skills/pantarhei-solve/references/catalog.json` format (schema: `pantarhei-core/schema/method.schema.json`).

Rules for every record:

1. Own words. No sentence copied from the source; the validator blocks quoted spans over 14 words and 8-word overlaps with known source lists.
2. Credit the originator in `origin` with author, work and year, and a URL to the publisher or author page.
3. Pick the evidence class honestly: `formal`, `empirical`, `heuristic` or `analogical`. It caps what the skill may claim.
4. Do not use trademarked method names (see `pantarhei-core/tests/trademarks.txt`).
5. Run `python .core/scripts/validate.py --root .` before opening the pull request.
