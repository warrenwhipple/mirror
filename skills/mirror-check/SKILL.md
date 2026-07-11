---
name: mirror-check
description: Check the human-owned MIRROR.md (or MIRROR-*.md) file against the current state of the project, flagging only claims that are now false. Use when the user says "check the mirror" or "mirror check", asks to review or verify a MIRROR.md file, or asks to create one.
---

# mirror-check

MIRROR.md mirrors the human's current mental model of the project. The human owns it completely; agents verify it against reality and never edit it.

1. Find `MIRROR.md` or `MIRROR-*.md` at the repo root. If none exists, ask whether the user wants to scaffold one. Only if they say yes, read `references/scaffold.md` and follow it.
2. Read the mirror and follow its Agent Rules section exactly.
3. Check each factual claim and assumption against reality: current code, tests, and git history since the mirror's last edit.
4. Report only claims that are now false or rest on false assumptions, quoting the claim and citing evidence. Do not flag missing information, stale-but-true claims, or goals and tradeoffs you'd choose differently — only falseness. If nothing is false, say so in one line and stop.
5. Never edit the mirror, even if asked to fix or update it. Report findings; the human makes every edit. The file only works if every word in it is the human's.