# NEXT_ACTIONS (AAHP)

## Status Summary

| Status  | Count |
|---------|-------|
| Done    | 19    |
| Ready   | 1     |
| Blocked | 0     |

---

## Ready - Work These Next

### T-019: T-002: Graceful file init - auto-create TODO.md if missing [medium]
- **Goal**: Close GitHub issue #2 - feature already implemented
- **Context**: Auto-creation of TODO.md was implemented in T-002. The `ensureTodoFile()` function creates the file with a default template if it does not exist, and `readTodoFile()` calls `ensureTodoFile()` before reading.
- **What to do**: Verify implementation in `index.ts` (lines 19-24, 26-29), confirm tests cover it, close GitHub issue #2, mark T-019 done in MANIFEST.json
- **Files**: `.ai/handoff/MANIFEST.json`, `index.ts`
- **Definition of done**: GitHub issue #2 closed, T-019 marked done

---

## Blocked

_No blocked tasks._

---

## Recently Completed

| Task   | Title                                              | Completed  |
|--------|----------------------------------------------------|------------|
| T-018  | T-003: Make section headers configurable           | 2026-02-28 |
| T-017  | T-004: Add TypeScript build configuration          | 2026-02-28 |
| T-016  | T-005: Add unit tests for core parsing/mutation    | 2026-02-28 |
| T-015  | T-006: Add /todo-edit command                      | 2026-02-28 |
| T-014  | T-007: Add /todo-remove command                    | 2026-02-28 |
