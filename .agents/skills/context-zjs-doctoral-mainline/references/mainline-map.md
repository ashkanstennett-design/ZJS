# Doctoral mainline map

Use this map to connect individual tasks without overstating their maturity.

| Layer | Core question | Typical inputs | Typical outputs | Link to next layer |
|---|---|---|---|---|
| Reservoir constraints | Under what geological and engineering conditions must stimulation work? | Petrel grids, facies, petrophysics, stress, pressure, completion constraints | Scenario set, spatial constraints, target envelopes | Defines loading, fluid, temperature, stress, geometry, and performance requirements for materials and fractures |
| Material mechanism | How do material microstructure and damage change conductivity? | Material composition and structure, loading path, fluid and thermal conditions, time-series experiments | Evolution laws, descriptors, uncertainty, failure modes | Supplies physically interpretable parameters and priors to fracture-scale models |
| Fracture scale | How do material laws manifest in a rough, closing, flowing fracture? | Aperture and roughness, proppant or material distribution, stress path, coupled flow-mechanics conditions | Effective conductivity, damage or closure response, upscaled parameters | Supplies response functions or reduced parameters for reservoir-scale prediction |
| Multiscale prediction | Can material-fracture-reservoir response be predicted quickly and robustly? | Curated cross-scale dataset, physical descriptors, scenario labels, simulation and experimental outputs | Surrogate models, uncertainty, sensitivity, feasible design space | Enables rapid screening and optimization under reservoir constraints |
| Selection and inverse design | Which material should be used, or what material properties are required, for a reservoir condition? | Reservoir requirement, operational constraints, objectives, uncertainty, candidate/design variables | Ranked choices, Pareto trade-offs, inverse-design targets, validation plan | Returns testable material designs and experiments, closing the loop |

## Evidence maturity labels

Use the narrowest label supported by the work:

- **Observed:** directly measured or recorded, with conditions and provenance.
- **Interpreted:** mechanism inferred from observations, with alternatives acknowledged.
- **Calibrated:** model parameters fitted within a stated domain.
- **Predicted:** model output for a specified domain and uncertainty.
- **Validated:** tested against data not used in fitting or training, under stated conditions.
- **Recommended:** engineering choice based on objectives, constraints, and uncertainty.

## Task framing card

For a new related task, answer compactly:

- Mainline layer and scale:
- Research question or decision:
- Inputs and evidence status:
- Output and acceptance check:
- Upstream dependency:
- Downstream use:
- Main uncertainty or missing validation:

## Cross-scale handoff checks

- Are variables physically meaningful and their units consistent?
- Are laboratory boundary conditions mapped to fracture or reservoir conditions?
- Is the representative scale or averaging rule explicit?
- Are model parameters identifiable rather than merely fitted?
- Is uncertainty propagated rather than erased at the next scale?
- Is extrapolation outside tested conditions visible?
- Can the final recommendation be traced back to reservoir requirements and supporting evidence?
