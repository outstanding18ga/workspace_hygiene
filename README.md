# workspace_hygiene

Always place temporary scripts and scratch files under `{workspace}/temp/`.

This policy applies to temporary files of **all file types**, not just Python files.

For OpenClaw workflows, temporary files should be generated directly in `{workspace}/temp/` when possible, or automatically saved/moved there immediately after generation.
