---
name: context-zjs-doctoral-mainline
description: Use for ZJS's personal doctoral research tasks related to unconventional-reservoir fracturing, multiscale material behavior, modeling, prediction, or optimization.
---

# ZJS doctoral mainline context

Apply this skill to the user's doctoral research and related deliverables. Do not force unrelated tasks into this framework.

More-specific applicable context takes precedence for working conventions; levels to the left take priority.

**Individual (this skill)** > Team > Business unit > Company > Default

## Research identity

The user is a first-year direct-entry PhD student in Petroleum and Natural Gas Engineering at Southwest Petroleum University. Treat them as an early-career researcher building a coherent, publishable research system, not as a beginner who needs technical content diluted.

## Mainline

Keep this causal and engineering chain intact:

1. Center the work on stimulation of unconventional reservoirs by hydraulic fracturing.
2. Use Petrel to establish reservoir models and geological and engineering constraints.
3. Use fracturing-material experiments to reveal how material microstructure, damage, and conductivity evolve.
4. Use fracture-scale models to transfer mechanisms and parameters across scales.
5. Use machine learning for fast multiscale prediction and optimization across material, fracture, and reservoir levels.
6. Deliver reservoir-condition-oriented material selection and inverse design.

Read [references/mainline-map.md](references/mainline-map.md) when framing a research question, designing an experiment or model, planning a paper or thesis chapter, or judging whether a result closes a link in the chain.

## Working rules

- Locate each related task in the mainline and state the upstream inputs, downstream decision, and scale involved.
- Preserve the user's requested deliverable. A task may strengthen only one link; it does not need to cover the entire chain.
- Prefer outputs that connect mechanisms to engineering decisions. Record units, boundary conditions, sample or spatial scale, data provenance, uncertainty, and validation route when they matter.
- Separate experimental observation, interpreted mechanism, model assumption, calibrated parameter, machine-learning prediction, and engineering recommendation. Do not present one as another.
- Treat Petrel outputs as reservoir and constraint models until data coverage, geometry, units, calibration, and uncertainty are checked. Do not present a first-pass property model as a field conclusion.
- Treat AI-generated visuals and synthetic data as explanatory or methodological assets, never as experimental or field evidence.
- When proposing machine learning, define the target, features, sample unit, split strategy, leakage controls, uncertainty, physical constraints, and an external or cross-condition validation plan.
- Prefer research tasks that make adjacent scales interoperable: material descriptors to fracture parameters, fracture parameters to reservoir response, and reservoir requirements back to material design variables.
- Flag scope drift when a task is technically interesting but does not support the mainline, a required method, or a defensible publication outcome.

## Reusable skill distillation

After completing a substantive mainline-related task, assess whether it produced non-obvious reusable value. Create or update a repository-local skill only when at least one item can be reused: a validated workflow, stable decision rule, data schema, calculation or script, quality-control checklist, template, or recurring failure-and-recovery pattern.

When distillation is warranted:

1. Put the skill under `.agents/skills/<lowercase-hyphenated-name>/`.
2. Keep `SKILL.md` concise and specify when it applies and when it does not.
3. Preserve exact inputs, outputs, units, assumptions, evidence boundaries, verification steps, and stopping conditions that materially affect correctness.
4. Put detailed domain notes in `references/`, deterministic repeated logic in `scripts/`, and reusable output materials in `assets/` only when needed.
5. Link to source artifacts instead of copying large raw datasets, private records, or one-off outputs into the skill.
6. Validate the skill with the available `skill-creator` validator and update the repository `SKILL_INDEX.md`.

Do not create a skill for trivial edits, one-off facts, unverified hypotheses, or a workflow that has not yet produced reliable evidence. Local commits are allowed when the user asks for repository persistence; pushing to a remote or publishing externally still requires explicit authorization.
