# orchestrator-specs-sample

Neutral-org **product specs repo** for the [Specfuse Orchestrator](https://github.com/clabonte/orchestrator) walkthroughs. Paired with [`orchestrator-api-sample`](https://github.com/Bontyyy/orchestrator-api-sample) and [`orchestrator-persistence-sample`](https://github.com/Bontyyy/orchestrator-persistence-sample) as the component repos those walkthroughs target.

## Layout

- `/product/` — agent-accessible product specs.
  - `features/` — per-feature acceptance criteria files, one per `FEAT-YYYY-NNNN`. Authoritative behavior contract for each feature; enumerated against by the QA agent's `qa-authoring` skill when drafting a test plan.
  - `test-plans/` — per-feature test plans emitted by the QA agent's `qa-authoring` skill. One file per feature, YAML frontmatter shape governed by [`test-plan.schema.json`](https://github.com/clabonte/orchestrator/blob/main/shared/schemas/test-plan.schema.json).
- `/business/` — non-agent-accessible (brand, marketing, support). Intentionally empty in this sample; present so the orchestrator's `never-touch` boundary is meaningful.

## Provenance

Stood up during Work Unit 3.6 of the orchestrator implementation plan — the Phase 3 walkthrough. Phase 0 WU 0.8 had deferred the product-specs-repo setup; WU 3.6 effectively required it, so the repo is created here and the deferral is recorded as a retrospective input in WU 3.7.

## License

Apache 2.0. See [LICENSE](LICENSE).
