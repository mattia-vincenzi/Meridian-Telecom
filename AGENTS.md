# Meridian Telecom Take-Home

## Purpose

This repository is used to prepare the Meridian Telecom Platform Engineer take-home assignment.

The objective is to produce a coherent, pragmatic and defensible solution for the technical discussion.

Do not optimize for completeness or architectural sophistication.

## Source of truth

Before doing any substantial work:

1. Read `assignment.md` in full.
2. Treat `assignment.md` as the authoritative source of requirements and constraints.
3. Read `solution.md` to understand the current working proposal.

Do not duplicate the assignment into other documents.

Do not silently convert assumptions into requirements.

Always distinguish between:

* explicit requirements;
* assumptions;
* design decisions;
* unresolved questions.

## Working approach

Prefer the simplest solution that credibly satisfies the assignment.

Avoid unnecessary architecture, services and abstractions.

Do not introduce a technology merely because it is common or considered a best practice.

For material decisions:

* explain the problem being solved;
* identify credible alternatives;
* explain why the proposed option was selected;
* make the important trade-offs explicit;
* state what could cause the decision to be revisited.

Consider the initial workload and the stated growth path, but avoid building final-scale complexity prematurely.

## Critical review

Do not simply agree with the current proposal.

Actively challenge:

* unnecessary complexity;
* premature optimization;
* unclear ownership;
* hidden failure modes;
* weak recovery semantics;
* assumptions presented as facts;
* operational burden that is disproportionate to the team;
* cost or lock-in without a clear benefit.

When challenging a decision, provide a credible alternative and explain its trade-offs.

Avoid criticism that does not materially affect the design.

## Missing information

When the assignment does not provide enough information:

1. identify the uncertainty;
2. explain whether it materially affects the design;
3. make a reasonable working assumption when needed;
4. record important assumptions in `solution.md`.

Do not invent precise workload, latency, traffic or cost numbers without evidence.

## Level of detail

This is preparation for an approximately 30-minute technical presentation, not a production implementation or full system design specification.

Prioritize the decisions that are worth discussing and defending.

Prefer a small number of well-reasoned decisions over exhaustive implementation detail.

Do not create additional documentation or artifacts unless they materially improve the final presentation or reasoning.

## Working document

Use `solution.md` as the main working document.

Keep it concise and focused on:

* requirements and constraints that drive the design;
* assumptions and open questions;
* proposed architecture;
* key decisions and trade-offs;
* reliability, security and operability;
* scaling and cost;
* delivery roadmap;
* AI usage.

Do not modify `assignment.md` unless explicitly asked.

## AI usage

Maintain enough factual notes in `solution.md` to later explain:

* which AI tools or models were used;
* what work was delegated;
* important suggestions that were accepted;
* important suggestions that were rejected or substantially changed;
* how the work was reviewed and validated.

Do not fabricate or reconstruct AI usage retrospectively.
