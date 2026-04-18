---
name: workspace_hygiene
description: Always place temporary scripts and scratch files under {workspace}/temp.
---

Use this skill whenever writing any temporary file, scratch file, intermediate output, or one-off script.

Temporary files include:
- tmp_*.py
- tmp_*.js
- scratch scripts
- intermediate text/json/csv outputs
- one-off helper scripts created only to complete the current task

Never write temporary files to the workspace root.

Always write temporary files under:

{workspace}/temp/

Only reusable, permanent, or user-requested deliverables may be written outside {workspace}/temp/.