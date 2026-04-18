---
name: workspace_hygiene
description: Always place temporary scripts and scratch files under {workspace}/temp.
---

Use this skill whenever writing any temporary file, scratch file, intermediate output, or one-off script.

Temporary files include (but are not limited to):
- `tmp_*.py`, `tmp_*.js`, `tmp_*.ts`, `tmp_*.sh`
- scratch scripts in any language
- intermediate `.txt`, `.md`, `.json`, `.yaml/.yml`, `.csv`, `.log` outputs
- generated artifacts such as temporary configs, SQL files, notebooks, or data extracts
- one-off helper scripts created only to complete the current task

Never write temporary files to the workspace root (or any non-temp project directory).

Always write temporary files under:

`{workspace}/temp/`

## OpenClaw temp-file behavior

When OpenClaw generates temporary content, it must be persisted automatically to the temp directory.

Preferred behavior:
1. Generate the temporary file directly under `{workspace}/temp/`.
2. If generation happens elsewhere first, immediately move/save it to `{workspace}/temp/` as part of the same workflow step.

Do not leave generated temporary files unsaved or outside `{workspace}/temp/`.

Only reusable, permanent, or user-requested deliverables may be written outside `{workspace}/temp/`.
