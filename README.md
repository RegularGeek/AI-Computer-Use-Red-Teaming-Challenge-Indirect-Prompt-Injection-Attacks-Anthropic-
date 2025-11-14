# Computer Use Red Teaming Challenge — Repository

**Purpose:** A safe, professional scaffold for documenting and submitting your red-team research on the Anthropic "Computer Use" agent. This repo intentionally contains *placeholders only* and **no exploit payloads**. Use local copies (not committed) for any active testing artifacts.

## Contents
- `docs/` — methodology, report template, ethics & legal, screenshots folder.
- `infrastructure/harmless_site/` — safe HTML placeholder representing a user-generated content area.
- `artifacts/` — (ignored) place evidence here locally; do not commit secrets.
- `packaging/` — scripts and instructions to prepare the ZIP for Mindrift.
- `.github/` — issue and PR templates.

## Quick start
1. Extract the ZIP and inspect files.
2. Keep any exploit payloads & secrets **offline** in a private working directory.
3. Follow `docs/METHODOLOGY.md` and `packaging/make_zip.sh` to prepare submission.

## Safety & compliance (short)
- DO NOT commit API keys, private data, or exploit code.
- Evidence files (screenshots, recordings) must be redacted before upload.
- This repo is for documentation and reproducibility; active testing must be performed in the supplied test environment only.

## How to run the harmless demo site locally
```bash
cd infrastructure/harmless_site
# Python 3
python -m http.server 8000
# Then open http://localhost:8000 in your browser
```

## GitHub upload
See `packaging/github_push_instructions.md` for step-by-step commands including recommended `.gitignore` entries and branch workflow.

## What's next
- Use `docs/METHODOLOGY.md` to record your test plan and final results.
- Use `packaging/make_zip.sh` to create a final submission ZIP for Mindrift.
