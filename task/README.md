# README: tasky.overlord.md

## TASKLIST FORMAT — AGENT REFERENCE

## Core Mechanic

`[id]:TODO[ ]` is intentionally invalid markdown reference syntax. A valid markdown reference requires a URL: `[id]:https://...`. `TODO[ ]` is not a URL — it is a syntax error by design.

**Invalidity = incomplete. Validity = complete. They are the same event.**

> Inserting `x` into the brackets (`TODO[ ]` → `TODO[x]`) corrects the syntax.
> IncompleteTask: syntax_error | completeTask: syntax_correct
> Essentially, a completed task also corrects the syntax, providing a verifiable, structured tasklist. An agent or editor can detect completion state by testing reference validity alone.

`[>]` is also invalid. Blocked tasks remain syntactically broken, distinguishable from incomplete only by the character.

The preferred completion act replaces `TODO[x]` entirely with a real artifact reference:

```md
[01]:TODO[ ]                                       ← incomplete, invalid
[01]:TODO[x]                                       ← complete, valid (minimum)
[01]:https://github.com/org/repo/commit/abc123     ← complete, valid, navigable
```

When a real reference is used, `[01]` in the prose block resolves as a live link. Completion creates traceability.

---

## Structure

```md
# REQUIREMENTS

> {insight_block}               ← scoped context required to execute tasks correctly

## TODO

- [{id}] {task} | {rationale}   ← prose definition, id is the index key

---

[{id}]:TODO[ ]                  ← state index, authoritative completion record

---
```

## State Index

| Syntax               | State             | Valid Markdown |
|----------------------|-------------------|----------------|
| `[id]:TODO[ ]`       | incomplete        | no             |
| `[id]:TODO[>]`       | blocked           | no             |
| `[id]:TODO[x]`       | complete          | yes            |
| `[id]:{url_or_path}` | complete + linked | yes            |

## Rules

- Index is authoritative. Prose is context. Do not conflate.
- `[id]` in prose and `[id]:` in index are the same key. They are coupled.
- Transition `TODO[ ]` → `TODO[x]` is the minimum completion act.
- Transition `TODO[ ]` → `{artifact}` is preferred when a commit SHA, file path, or URL exists.
- `TODO[>]`(blocked) agent requires user intervention, cannot complete tasks. Infer resolution.
- Index entries are processed in order unless a dependency or blocked state requires otherwise.
- Do not reorder index entries. Do not renumber. IDs are stable references.
- Insight block is scoped context for this task set only. Do not generalize beyond it.

---
