# OVERLOLD MAP PRIMER
Contextual onboarding and operational reading guide for `map.overlord.yaml`

---

## PURPOSE

`rules.overlord.rs` teaches the agent **how OVERLORD thinks**, then `map.overlord.yaml` teaches the agent:
- where authority lives,
- how repository files are ranked,
- how records are shaped,
- how truth flows through the codebase,
- when to stop,
- when to shard,
- how to validate,
- how to evolve the protocol safely.

This README is not the protocol itself.

It is the minimal onboarding guide required so an agent does not misread the YAML as generic project metadata instead of what it actually is:

**a canonical repository mapping contract for agent execution.**

---

## PRIMARY DIRECTIVE

`map.overlord.yaml` is a **canonical runtime mapping file**.

It is:
- operational,
- authoritative,
- ordered,
- schema-bearing,
- repository-aware,
- strict in interpretation,
- designed for agent runtime use.

It is not:
- casual repository notes,
- a loose manifest,
- a convenience file,
- a documentation mirror,
- a brainstorming structure.

The agent must read it as a **control contract**.

---

## RELATION TO `rules.overlord.rs`

The two files serve different but connected purposes.

### `rules.overlord.rs`
Defines:
- agent alignment,
- pseudo-Rust symbolic behavior,
- truth boundaries,
- output discipline,
- safe completion behavior.

### `map.overlord.yaml`
Defines:
- runtime execution order,
- file authority hierarchy,
- repository role mapping,
- record schemas,
- inference policy,
- validation rules,
- scaling rules,
- protocol change discipline.

The correct relationship is:

- `rules.overlord.rs` defines the **agent reading and execution posture**
- `map.overlord.yaml` defines the **repository execution map and canonical runtime contract**

Do not merge their purposes.
Do not flatten one into the other.

---

## WHAT `map.overlord.yaml` IS

`map.overlord.yaml` is the repository’s **canonical contextual mapping layer**.

It tells the agent:
- what the repository root assumptions are,
- which files are canonical,
- which files are advisory,
- which files are mirrors,
- which files are non-canonical,
- what order to parse sections in,
- how authority conflicts resolve,
- what record schemas are valid,
- what evidence promotion is allowed,
- what validation failures stop writes,
- when scaling/sharding activates,
- how protocol change must be managed.

It is closer to:
- a runtime contract,
- a repository governance map,
- a truth routing file,
- a canonical execution schema,

than to ordinary configuration.

---

## WHAT THE FORMAT OPTIMIZES FOR

The YAML map is optimized for:

1. **Context Precision**
   - exact file role awareness,
   - exact authority ranking,
   - exact target resolution.

2. **Retrieval Efficiency**
   - reduced search drift,
   - fast file-class identification,
   - explicit source ordering.

3. **Traceability**
   - records tied to schemas,
   - evidence tied to claims,
   - links tied to rationales,
   - authority tied to file roles.

4. **Update Consistency**
   - stable schema expectations,
   - explicit change control,
   - controlled sharding rules,
   - non-silent conflict behavior.

5. **Agent Runtime Safety**
   - stop conditions,
   - fail actions,
   - non-canonical containment,
   - unresolved conflict detection.

---

## WHAT THE FORMAT DOES NOT OPTIMIZE FOR

The map is not primarily trying to be:
- a human tutorial,
- a prose design essay,
- a lightweight informal note,
- optional guidance,
- approximate metadata.

It is meant to be read strictly.

Do not weaken its meaning into “helpful hints.”

---

## CORE INTERPRETATION MODEL

An agent must read `map.overlord.yaml` top to bottom, as declared by the protocol itself.

The file explicitly states:

- `mode: yaml_canonical`
- `parse_strategy: strict_top_to_bottom`

This is not advisory.

This means the agent should:
1. parse in the declared order,
2. preserve section meaning,
3. not skip ahead casually,
4. not reinterpret later sections before earlier authority is understood,
5. not apply schemas before reading truth precedence and execution behavior.

The YAML is ordered for a reason.

---

## FIRST PRINCIPLE OF SAFE READING

The agent must assume:

- section order matters,
- field names matter,
- enum values matter,
- rejection conditions matter,
- conflicts are stopping events when defined as such.

The agent must not assume:
- a field is optional unless explicitly stated,
- a lower-authority file can fill a gap in a canonical file,
- inferred relations can complete canonical records,
- mirrors can override sources,
- historical files can steer present truth.

---

## HIGH LEVEL SECTION MAP

The protocol explicitly requires reading sections in this order:

1. `runtime_contract`
2. `file_role_authority_map`
3. `truth_precedence`
4. `execution_contract`
5. `lok_contract`
6. `record_schemas`
7. `source_and_inference_policy`
8. `validation_contract`
9. `scaling_contract`
10. `change_control`
11. `last_parse_retention_priority`

The agent must preserve this order in interpretation.

Each section has a distinct job.

---

## SECTION BY SECTION UNDERSTANDING

## 1. `runtime_contract`

This section defines how the entire YAML must be read.

It establishes:
- protocol identity,
- version,
- audience,
- invocation context,
- root requirements,
- parsing mode,
- parse order,
- optimization goals,
- reject conditions.

This section is the runtime handshake.

The agent should treat it as:
- the file’s self-declared operating contract,
- the highest local interpretation guide inside the YAML.

Important implications:
- repository root matters,
- section ordering matters,
- missing sections are rejection-worthy,
- unresolved authority conflicts are rejection-worthy.

This means an agent cannot safely “best effort” past structural protocol damage without explicitly surfacing that break.

---

## 2. `file_role_authority_map`

This section defines the repository’s file-class ontology.

It tells the agent:
- what each file is for,
- what authority it has,
- whether it is canonical,
- whether it is writable,
- whether it is advisory, mirror, historical, or governance class.

This section prevents file confusion.

Example semantic distinctions in the map:
- `OVERLORD.yaml` is canonical governance
- `OVERLORD.md` is a low-authority mirror
- research baseline docs are high authority
- prototype and translation artifacts are non-canonical
- archive material is lowest authority

The agent must use this map before interpreting a file’s weight.

Do not judge file importance by filename alone.

Use:
- `role`
- `class`
- `authority`
- `canonical`

as the actual weighting basis.

---

## 3. `truth_precedence`

This section defines global truth rank.

It tells the agent how to resolve authority between:
- current user instruction,
- OVERLORD protocol files,
- canonical research,
- non-canonical support material,
- associative inference.

This is one of the most important sections in the entire map.

It prevents:
- mirror override,
- support-doc inflation,
- inference-based promotion,
- silent conflict collapse.

The agent must preserve:

- lower rank number wins,
- same-rank unresolved conflict must be marked unresolved and must stop.

That last part matters.

Conflict is not permission to improvise.

---

## 4. `execution_contract`

This section defines request-handling expectations.

It tells the agent:
- what fields every request classification should include,
- what request types exist,
- what behaviors are hard rules,
- what conditions require stopping.

This section governs operational handling of real work.

The agent must respect:
- request structure,
- canonical promotion restrictions,
- source invention prohibition,
- status emission discipline,
- stop conditions.

This means the agent should not just perform a repository action.
It should first understand the request as a classified protocol event.

---

## 5. `lok_contract`

This section formalizes the repository’s layered knowledge model.

It defines required fields for:
- task alignment,
- navigation context,
- canonical records.

This is not optional structural decoration.

It is the agent’s expected knowledge decomposition model.

The agent should use it to separate:
- current task intent,
- repository navigation metadata,
- actual canonical record content.

The `mentions` split into:
- `direct`
- `associative`

is especially important.

Do not collapse these.

That split preserves semantic cleanliness and prevents fuzzy graph contamination.

---

## 6. `record_schemas`

This section defines the system’s real schema shapes.

It tells the agent:
- valid id patterns,
- required metadata fields,
- claim record requirements,
- evidence record requirements,
- link record requirements,
- allowed enums,
- status values.

This is the schema backbone of the repository map.

The agent must treat these as validation-critical expectations.

If editing, transforming, or generating structured records, the agent must preserve:
- field presence,
- id discipline,
- enum legality,
- canonicality distinction,
- mention structure,
- source linkage.

Do not freestyle around this section.

---

## 7. `source_and_inference_policy`

This section governs evidence quality and allowable reasoning.

It tells the agent:
- what source tiers exist,
- what evidence strength is needed for canonical stable claims,
- what tier-C-only material is allowed to become,
- what inference types are allowed,
- what inference types are forbidden.

This is the anti-fabrication and anti-overreach section.

It is crucial because it limits how far the agent can go even when a pattern seems useful.

Important implications:
- not all evidence is equal,
- tier-C-only support cannot become stable canonical truth,
- association alone cannot justify canonical promotion,
- structural inference is allowed only within scoped limits.

This section should be read as a permission boundary, not a suggestion.

---

## 8. `validation_contract`

This section defines required pass checks and failure behavior.

It tells the agent what must be true before a result is considered valid.

Required pass checks include:
- no fabricated sources,
- no dangling IDs,
- no missing status,
- no missing source of truth in claims,
- mention split integrity,
- authority-map compliance,
- truth precedence compliance.

Failure actions include:
- mark unresolved,
- emit gap record,
- stop writes for canonical targets.

This means validation failure is not just a note.
It changes write behavior.

The agent must not continue canonical writes after failing the declared validation contract.

---

## 9. `scaling_contract`

This section defines when the system must shard.

It tells the agent:
- what thresholds activate scaling,
- what shard targets exist,
- what invariants must survive sharding.

This is for repository growth control.

The agent must preserve:
- full schema shape,
- stable record IDs,
- origin pointers.

Sharding is not a redesign.
It is a controlled scaling response.

---

## 10. `change_control`

This section defines protocol evolution discipline.

It tells the agent what must happen when the protocol changes.

Important requirements include:
- version increment,
- change summary inclusion,
- breaking-change flagging,
- migration steps,
- backward ID preservation,
- no renaming IDs through mutation.

This section exists so the protocol can evolve without corrupting continuity.

The agent must treat protocol changes as governed events, not casual edits.

---

## 11. `last_parse_retention_priority`

This section defines continuous refinement retention and feedback capture.

It tells the agent that:
- refinement is mandatory,
- learning from parse outcomes matters,
- what failed must be retained,
- retrieval failures matter,
- ambiguity events matter,
- growth trends matter,
- spec changes should be tested and measured.

This section is effectively the protocol’s self-improvement memory discipline.

It prevents terminal complacency.

This means the system is designed to refine itself continuously, but in a controlled and evidence-aware way.

---

## FILE AUTHORITY MODEL

The map’s authority handling is one of its central functions.

The agent must reason about files through these axes:

- `role`
- `class`
- `authority`
- `canonical`
- `writable`

These do not mean the same thing.

### `role`
What the file is for.

### `class`
What functional category it belongs to.

### `authority`
How much truth-weight it carries.

### `canonical`
Whether it is part of the truth-bearing source core.

### `writable`
Whether modifications are allowed.

A file may be writable and still non-canonical.
A file may be canonical and still not outrank user instruction.
A mirror may resemble source truth but still remain low authority.

The agent must keep these distinctions explicit.

---

## REQUEST HANDLING MODEL

When performing work under this YAML, the agent should internally classify the task with at least:

- `request_id`
- `request_type`
- `target_files`
- `target_authority_class`
- `expected_output_type`

This is the runtime framing expected by the map.

Even if the user does not provide these labels explicitly, the agent should reason in that structure when applying the protocol.

The allowed request types currently include:
- `review`
- `transform`
- `link`
- `normalize`
- `update`
- `validate`

The agent should avoid unclassified action logic where a defined request class already exists.

---

## CANONICALITY MODEL

The YAML makes a hard distinction between canonical and non-canonical material.

The agent must preserve this distinction.

Canonicality affects:
- truth weight,
- promotion rules,
- write safety,
- conflict consequences,
- validation strictness.

The agent must never:
- silently promote non-canonical content,
- treat support artifacts as canonical because they are detailed,
- use associative inference as canonical evidence,
- overwrite canonical claims without explicit authority.

Canonicality is protocol-governed, not convenience-governed.

---

## EVIDENCE MODEL

The repository uses evidence-bearing records, not unsupported assertions.

The agent must understand:

### claim records
Contain:
- statement-level research claims,
- their canonicality,
- evidence links,
- truth source,
- mentions,
- status,
- revision.

### evidence records
Contain:
- source classification,
- citation,
- source location,
- extraction note,
- verification state,
- status.

### link records
Contain:
- graph relation between records,
- rationale,
- status.

The agent must treat these as interlocking structures.

A claim without evidence discipline is not structurally complete under this map.

---

## INFERENCE MODEL

Inference is allowed, but tightly scoped.

The YAML permits:
- structural inference from explicit text,
- direct link extraction from explicit references,
- associative link extraction with non-canonical labeling.

The YAML forbids:
- unsupported claim creation,
- source fabrication,
- canonical promotion from association only.

This is critical.

The agent is allowed to reason.
The agent is not allowed to convert reasoning into unsupported authority.

Inference is subordinate to source.

---

## VALIDATION MODEL

Validation is not advisory.

Before considering output safe, the agent must ensure:
- no fabricated sources,
- no broken IDs,
- no absent statuses,
- no missing source-of-truth field in claims,
- no collapsed mention split,
- no authority map violations,
- no truth precedence violations.

If these fail:
- unresolved marking is required,
- gap emission may be required,
- canonical writes must stop.

This means the protocol is willing to preserve incompleteness rather than allow corrupted certainty.

That is a core design strength.

---

## SCALING MODEL

When thresholds are exceeded, the system activates sharding.

This matters because an agent must not keep expanding a single-file architecture past defined scaling points.

The agent should watch:
- record counts,
- source counts,
- cross-document link counts.

When scaling triggers, the agent should use the designated shard targets while preserving:
- schema shape,
- IDs,
- origin traceability.

Growth does not justify schema drift.

---

## CHANGE MODEL

When modifying the protocol itself, the agent must respect change control.

This means:
- protocol version changes must be explicit,
- change summaries must exist,
- breaking changes require migration steps,
- ID continuity must be preserved,
- deprecate-and-replace is preferred over rename mutation.

The agent must not edit the protocol as if it were ordinary content.

Protocol edits are governance events.

---

## PARSE RETENTION MODEL

The final section establishes that continuous refinement is mandatory.

The agent must treat:
- retrieval failures,
- ambiguity events,
- unresolved growth trends,
- what worked,
- what failed

as important retained signals for future refinement.

This means the map is not static governance.
It is adaptive governance with controlled feedback.

The agent should preserve that spirit:
- refine by evidence,
- test translation on one file,
- measure delta,
- keep or revert intentionally.

---

## WHAT AN AGENT MUST NOT DO

When using `map.overlord.yaml`, do not:

- treat section order as optional,
- use low-authority files to override canonical files,
- ignore stop conditions,
- continue canonical writes after validation failure,
- silently resolve same-rank conflicts,
- promote associative inference to canonical truth,
- generate records that violate required schema fields,
- mutate IDs casually,
- treat mirrors as authoritative sources,
- interpret the file as descriptive only.

---

## WHAT AN AGENT SHOULD DO

When applying this map, the agent should:

- parse top to bottom in declared order,
- establish repository-root context first,
- identify file authority before reading content weight,
- resolve truth precedence before performing updates,
- classify requests structurally,
- preserve LOK separation,
- enforce record schemas,
- keep inference scoped,
- validate before canonical write,
- stop when stop conditions are reached,
- respect sharding thresholds,
- preserve protocol continuity during change.

---

## SAFE OPERATIONAL CHECKLIST

Before acting under `map.overlord.yaml`, the agent should confirm:

- I am treating this as canonical runtime mapping.
- I know the parse order.
- I know which files are canonical vs advisory vs historical.
- I know the truth precedence stack.
- I know whether my target files are writable.
- I know my request classification.
- I know the required schema for the records I am touching.
- I know what inference is allowed.
- I know what validation failures block canonical writes.
- I know whether scaling/sharding rules apply.
- I know whether my change would require protocol version discipline.

If any of these are false, the agent is not ready to operate safely under the map.

---

## BAD INTERPRETATION EXAMPLES

The agent must avoid these mistakes.

### Mistake 1
“This is just a repository inventory.”

Wrong because:
- it is a runtime and truth-governance contract.

### Mistake 2
“A detailed non-canonical support file can fill canonical gaps automatically.”

Wrong because:
- canonical promotion rules are explicit and restrictive.

### Mistake 3
“Validation failures can be noted and ignored if the overall output looks useful.”

Wrong because:
- fail actions include stopping canonical writes.

### Mistake 4
“Same-rank conflicts can be resolved by choosing the more detailed source.”

Wrong because:
- same-rank conflicts must be marked unresolved and stop.

### Mistake 5
“Section order is organizational only.”

Wrong because:
- strict top-to-bottom parsing is part of the protocol.

---

## GOOD INTERPRETATION MODEL

A correct agent reading sounds like this internally:

- This YAML is canonical runtime control, not casual metadata.
- Parse order matters.
- File role and authority must be known before content weighting.
- Truth precedence must be resolved before updates.
- Schemas are mandatory.
- Inference is limited and subordinate to source.
- Validation gates canonical writes.
- Scaling and change rules are operational, not decorative.
- Continuous refinement is expected, but must remain measured and controlled.

---

## FINAL UNDERSTANDING REQUIREMENT

The correct relationship between this README and `map.overlord.yaml` is:

- this README teaches the execution reading model,
- `map.overlord.yaml` carries the canonical repository mapping contract,
- repository operations must follow authority and validation discipline,
- inference must remain bounded,
- protocol refinement must remain governed.

The agent should leave this README with one core understanding:

**`map.overlord.yaml` is the canonical runtime map that tells the agent where truth lives, how structure is validated, and when execution must stop instead of guessing.**

---
