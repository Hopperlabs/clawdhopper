---
description: Save, restore, and list Claude Code sessions
disable-model-invocation: true
---

Manage the current session context. Based on the user's request, do one of:

**Save** - Save the current session state:
- Summarize what was accomplished so far
- Note key files modified, decisions made, and open tasks
- Write the summary to `.claude/sessions/<name>.md`

**Restore** - Restore a previous session:
- Read the session file from `.claude/sessions/<name>.md`
- Present the summary and offer to continue where it left off

**List** - List available saved sessions:
- Glob `.claude/sessions/*.md` and display them with dates

Ask the user which action they want if not specified.