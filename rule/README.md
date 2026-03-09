# OVERLORD FORMAT PRIMER

Contextual onboarding and operational reading guide for `rules.overlord.rs`

---

## PURPOSE

This README exists to prepare an agent to correctly read, interpret, and apply the `rust.overlord` pattern format used in `rules.overlord.rs`.

This file is the first contextual onboarding file.

Its job is not to replace `rules.overlord.rs`.

Its job is to ensure the agent does **not**:
- misread the format as normal Rust,
- flatten the format into default prose policies,
- invent missing semantics,
- over-prioritize rhetorical language over operational rules,
- confuse inferred relations with validated authority.

This README establishes the minimum required understanding for safe and useful interaction with the OVERLORD rules format.

---

## PRIMARY DIRECTIVE

`rules.overlord.rs` is a **custom pseudo-Rust pattern language**.

It is:
- pattern based,
- intentionally syntax-adjacent,
- designed for repeated agent scanning,
- optimized for contextual alignment,
- not intended to be valid Rust,
- not intended to be compiled,
- not intended to be judged by Rust parser rules.

The host syntax resemblance exists for:
- structural familiarity,
- visual grouping,
- markdown code fence highlighting,
- symbolic consistency,
- dense agent-readable pattern anchors.

The correct task is to interpret the format **as designed**, not to normalize it into a generic rule document.

---

## WHAT `rules.overlord.rs` IS

`rules.overlord.rs` is an agent rules file that defines:
- alignment principles,
- execution standards,
- truth boundaries,
- status discipline,
- output behavior,
- authority precedence,
- pattern interpretation rules.

It is a control surface for repeated agent re-alignment.

It is not a complete project archive.

It is not a general essay.

It is not a normal coding standards file.

It is not a substitute for repository source truth.

It is a **high-frequency alignment file**.

---

## WHAT THE FORMAT OPTIMIZES FOR

The OVERLORD format is designed to balance the following:

1. **Pattern Recognition**
   - repeated symbolic shapes,
   - stable semantic anchors,
   - predictable grouping.

2. **Scan Efficiency**
   - fast repeated review,
   - low narrative drift,
   - compact rule presentation.

3. **Contextual Guidance**
   - operational alignment,
   - quality enforcement,
   - truth preservation,
   - scoped inference.

4. **Pseudo-Formal Structure**
   - stronger than prose,
   - lighter than a fully formal grammar,
   - structured enough for machine-like reading,
   - flexible enough for evolving documentation.

5. **Assumption Safety**
   - no fabrication,
   - no silent authority escalation,
   - no false completion,
   - no confusion between inferred and validated data.

---

## WHAT THE FORMAT DOES NOT OPTIMIZE FOR

The format is **not** primarily designed for:
- Rust correctness,
- compiler acceptance,
- academic prose elegance,
- conventional configuration syntax,
- strict JSON/YAML serialization,
- automatic execution,
- decorative stylistic mimicry.

Do not judge it by those standards.

---

## INTERPRETATION MODEL

An agent reading `rules.overlord.rs` must treat it as a **semantic pattern system**.

The reading model is:

1. identify the block type,
2. identify the purpose of the block,
3. identify the active rule class,
4. distinguish values from constraints,
5. distinguish authority from inference,
6. distinguish motivational emphasis from executional requirement,
7. preserve exact intent without translating it into default generic policy language.

The agent must read for:
- structure,
- rule class,
- authority level,
- truth boundary,
- output implications.

The agent must not read for:
- literal Rust execution,
- compiler repair,
- syntactic normalization,
- default documentation conventions.

---

## CORE FORMAT PRINCIPLE

The OVERLORD format is **syntax-shaped**, not syntax-bound.

That means:
- surface similarity to Rust is intentional,
- exact compliance with Rust is irrelevant,
- structural consistency matters more than language legality,
- recurring symbolic patterns carry semantic meaning.

The agent must preserve this principle in all transformations, edits, and extensions.

---

## MINIMUM SEMANTIC RULE

When reading the format:

- treat repeated structure as meaningful,
- treat labels as scope anchors,
- treat block names as semantic categories,
- treat strings as directive payload,
- treat declarations as relationship signals,
- treat higher authority blocks as stronger than stylistic or rhetorical force.

If uncertainty exists, preserve structure and mark uncertainty rather than rewriting into a safer-looking default format.

---

## HIGH LEVEL FORMAT MAP

The agent should expect the rules file to contain top-level sections such as:

- `#[OVERLORD::AGENT::ALIGNMENT]`
- `#[OVERLORD::AGENT::BOUNDARY]`
- `#[OVERLORD::AGENT::STATE]`
- `#[OVERLORD::AGENT::OUTPUT]`

These section headers are not decorative.

They indicate distinct semantic domains.

The agent must treat these domains as different classes of control:

### ALIGNMENT
Defines:
- operating posture,
- quality standards,
- contextual relevance,
- technical integrity,
- completion expectations.

### BOUNDARY
Defines:
- truth limits,
- inference limits,
- missing-context handling,
- conflict handling,
- authority precedence.

### STATE
Defines:
- explicit status language,
- safe output labeling,
- incompleteness handling,
- validation condition markers.

### OUTPUT
Defines:
- declaration consistency,
- scan readability,
- semantic weight discipline,
- pattern stability across reuse.

---

## BLOCK ELEMENTS AND HOW TO READ THEM

The agent should interpret common pattern elements as follows.

### 1. Section Header
Example shape:

```rs
#[OVERLORD::AGENT::ALIGNMENT]
````

Meaning:

- top-level semantic scope,
- defines the domain of the following rules,
- must influence interpretation of all enclosed declarations.

### 2. Documentation Comment Values

Example shape:

```rs
///! Values
///! V.1:"..."
```

Meaning:

- top-level explanatory or foundational statements,
- describes design philosophy,
- establishes intended reading discipline,
- provides high-level system values.

These are important, but they do not automatically override later explicit boundary rules.

### 3. Parameter Declaration

Example shape:

```rs
!param::Standards(BALANCE::FUNDAMENTAL::VALUES)
```

Meaning:

- activates or frames a rule family,
- defines the conceptual operating lens for the following block,
- acts as a typed semantic declaration.

### 4. Values Block

Example shape:

```rs
!values::Standards{ ... }
```

Meaning:

- compact validation map,
- key registration area,
- condensed system indexing of active values or states.

Read this as:

- a declaration of recognized internal anchors,
- not as executable language syntax,
- not as a JSON substitute.

### 5. Named Domain Array

Example shape:

```rs
ALIGNMENT: [ ... ]
```

Meaning:

- grouped operational domain,
- contains actual behavioral statements,
- often carries stronger execution implications than descriptive comments.

### 6. Scoped Entry

Example shape:

```rs
(a):comprehensive::EditRelativity()
```

Meaning:

- sub-rule identifier,
- local semantic anchor,
- narrow classification for the payload that follows.

### 7. Payload Assignment

Example shape:

```rs
EditRelativity = [
    "..."
]
```

Meaning:

- operative directive payload,
- the actual instruction body,
- should be interpreted as the executable semantic content of that entry.

---

## RULE STRENGTH DISCIPLINE

Not all lines carry equal force.

The agent must prioritize content in this order unless the rules file explicitly states otherwise:

1. explicit current user instruction,
2. explicit source-truth or authority-precedence rules,
3. boundary rules,
4. direct operational directives,
5. state rules,
6. output consistency rules,
7. descriptive values,
8. rhetorical emphasis.

This is important.

The agent must **not** allow:

- rhetorical intensity,
- identity posture,
- quality pressure,
- stylistic force

to override:

- truth boundaries,
- incomplete-context rules,
- source authority,
- explicit conflict handling.

---

## AUTHORITY MODEL

The agent must preserve authority order when interpreting or applying the format.

Default order:

1. current user instruction,
2. direct source data,
3. canonical definitions,
4. contextual associations,
5. inference.

This means:

- inference cannot outrank source truth,
- association cannot become canonical merely by being useful,
- completion pressure cannot justify invention,
- unresolved conflict must remain explicit.

If a lower-authority layer conflicts with a higher-authority layer, the higher-authority layer wins.

If same-level authorities conflict and no resolution rule exists, the conflict must be surfaced, not silently collapsed.

---

## ASSUMPTION SAFETY MODEL

The OVERLORD format is assumption-sensitive.

The agent must never:

- fabricate source content,
- invent completion,
- create fake continuity,
- silently promote inferred relations to validated truth,
- interpret missing data as permission to improvise canonical claims.

When context is incomplete, the agent should:

- preserve the structure,
- mark the limitation,
- label the state honestly,
- continue only within supported bounds.

Truthful partial completion is preferred over polished false completion.

---

## STATE DISCIPLINE

The agent must use explicit state thinking when interacting with the format.

Expected state categories may include:

- `DRAFT`
- `PARTIAL`
- `STABLE`
- `BLOCKED`
- `INFERRED`
- `VALIDATED`
- `DEPRECATED`

These states are not decorative tags.

They are control markers.

The agent must use them to reason about:

- certainty,
- readiness,
- authority,
- trust level,
- whether a claim is safe to extend.

---

## OUTPUT DISCIPLINE

When extending or modifying the format, the agent must preserve:

### Pattern Consistency

Equivalent meanings should use equivalent declaration shapes.

### Semantic Stability

Do not rename or reshape blocks casually if the semantic role remains the same.

### Scan Readability

The format is designed for repeated review.
Do not bloat it with generic explanatory prose.

### Density With Control

Compact output is good only if meaning stays precise.

### Rhetorical Containment

Motivational or emphatic lines must not dominate operational directives.

---

## WHAT AN AGENT MUST NOT DO

When handling `rules.overlord.rs`, do not:

- rewrite it into standard markdown policy format,
- convert it into normal Rust,
- “fix” syntax into Rust compliance unless explicitly requested,
- flatten pattern declarations into generic prose,
- remove symbolic structure because it looks unconventional,
- assume all caps means highest authority,
- assume descriptive values are more important than explicit boundary rules,
- infer missing authority precedence if a boundary block already defines it,
- optimize for conventional documentation aesthetics over system intent.

---

## WHAT AN AGENT SHOULD DO

When asked to review, extend, refine, or apply the format, the agent should:

- preserve pseudo-Rust pattern identity,
- maintain structural rhythm,
- improve semantic clarity without normalizing style,
- add missing bounded-truth behavior where needed,
- strengthen declaration consistency,
- clarify ambiguous operational blocks,
- separate validated vs inferred logic,
- preserve repeated-scan usability,
- respect the file as a contextual training and control layer.

---

## SAFE EXTENSION STRATEGY

When extending the format, the agent should follow this order:

1. identify the semantic domain,
2. determine whether the new content belongs in `ALIGNMENT`, `BOUNDARY`, `STATE`, or `OUTPUT`,
3. preserve existing declaration shape,
4. add only the minimum new symbolic structure needed,
5. ensure new directives do not conflict with authority rules,
6. ensure new completion language does not break assumption safety,
7. avoid decorative complexity.

A good extension strengthens the system without making the pattern language noisier.

---

## BAD INTERPRETATION EXAMPLES

The agent must avoid these reading mistakes:

### Mistake 1

“This is malformed Rust, so I should correct it.”

Wrong because:

- Rust validity is not the design goal.

### Mistake 2

“This is basically a normal rules file, so I should rewrite it as headings and bullets.”

Wrong because:

- the custom pattern language is the design.

### Mistake 3

“These strong completion statements mean I should fill in missing architecture.”

Wrong because:

- completion pressure is bounded by truth and authority rules.

### Mistake 4

“A useful inferred association can be treated as canonical.”

Wrong because:

- inferred and validated states must remain separate.

### Mistake 5

“Uppercase emphasis means absolute execution priority.”

Wrong because:

- semantic class outranks typography.

---

## GOOD INTERPRETATION MODEL

A correct agent reading sounds like this internally:

- This file is pseudo-Rust by design.
- Structural repetition is meaningful.
- I should preserve the symbolic pattern language.
- Boundary and authority rules constrain completion.
- State labels matter.
- I should not normalize away the custom format.
- I should improve clarity without removing identity.
- Partial truth is better than complete invention.

---

## OPERATIONAL CHECKLIST

Before acting on `rules.overlord.rs`, the agent should confirm:

- I understand this is not meant to compile.
- I understand the format is intentionally custom.
- I know which section I am reading.
- I can distinguish values from directives.
- I can distinguish directives from boundaries.
- I can distinguish inferred from validated content.
- I will preserve symbolic structure.
- I will not flatten this into default prose.
- I will keep authority precedence intact.
- I will not fabricate completion.

If any of these are false, the agent is not yet ready to modify the format safely.

---

## FINAL UNDERSTANDING REQUIREMENT

The correct relationship between this README and `rules.overlord.rs` is:

- this README teaches the reading model,
- `rules.overlord.rs` carries the operative pattern language,
- source truth and project files still outrank unsupported invention,
- the format must be preserved as a custom system,
- safe interpretation is more important than conventional formatting.

The agent should leave this README with one core understanding:

**OVERLORD is a custom symbolic alignment language, not a malformed version of a conventional one.**

---
