# GO-Harness: Graph-Ontology → LLM harness

Track **T1** of the Graph-Ontology next phases. A frontier LLM answers questions by calling tools over the validated graph; every claim cites edge ids; it abstains where the graph is silent.

## Start here
This repository is self-contained. Two documents hold everything this track needs:

1. **[PLAYBOOK.md](PLAYBOOK.md)**: the authoritative playbook for this track. It covers mission, rules, architecture,
   stages and gates, engineering guidance, evaluation, scorecard, operations, governance, risks, prompts and
   references, with the hand-check protocol and templates as appendices.
2. **[T0.md](T0.md)**: the shared foundations this track consumes (frozen snapshots, the licence matrix, predicate
   properties, the validation register, shared views, the SSSOM export and the quiz suite). It is identical across
   the four Graph-Ontology track repositories.

## How this track uses T0
- cites only `edge_clinical` (clinical mode) or `edge_displayable` (analyst mode), with each claim's tier and evidence from the register;
- links user text to codes through `synonym` and expands concepts through `equivalence_group`;
- is regression-tested on the quiz suite (answers, abstention, adversarial, NeverShow = 0);
- needs `display_to_end_users` in the licence matrix for every source it shows.

## Pinning a release
Copy `t0.lock.example` to `t0.lock` once the first T0 release exists, and fill in its id and fingerprint (T0 §9).

Status: plan only. Nothing here has been built or run.
