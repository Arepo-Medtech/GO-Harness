# GO-Harness: Graph-Ontology → LLM harness

Track **T1** of the Graph-Ontology next phases. A frontier LLM answers questions by calling tools over the validated graph; every claim cites edge ids; it abstains where the graph is silent.

## Start here
1. **[T0.md](T0.md)**: the shared foundations, identical in all four track repos (GO-Harness, GO-HGT, GO-PJI, GO-TS):
   frozen snapshots, the licence matrix, algebraic properties on predicates, the validation register, shared views,
   the SSSOM export and the quiz suite. This track consumes a T0 release; it never reads the live graph.
2. The full recipe for this track is in `COMPENDIUM.md` (track T1), in
   [Arepo-Medtech/graph-ontology-compendium](https://github.com/Arepo-Medtech/graph-ontology-compendium).
3. Method (rules R1–R17, validation layers L0–L6) is governed by `PLAYBOOK.md` in
   [Arepo-Medtech/one-shot](https://github.com/Arepo-Medtech/one-shot).

## How this track uses T0
- cites only `edge_clinical` (clinical mode) or `edge_displayable` (analyst mode), with each claim's tier and evidence from the register;
- links user text to codes through `synonym` and expands concepts through `equivalence_group`;
- is regression-tested on the quiz suite (answers, abstention, adversarial, NeverShow = 0);
- needs `display_to_end_users` in the licence matrix for every source it shows.

## Pinning a release
Copy `t0.lock.example` to `t0.lock` once the first T0 release exists, and fill in its id and fingerprint (T0 §9).

Status: plan only. Nothing here has been built or run.
