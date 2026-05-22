# demand-investigator-agent

An LLM agent that investigates demand-forecast anomalies in CPG retail data and produces plain-English root-cause reports. Built on real Walmart M5 sales data, with synthetic anomalies injected to validate the agent against ground truth.

**Status:** Week 0 of 4 — initial scaffolding in progress.

## What it does

When an anomaly is flagged, the agent autonomously queries related data sources, generates and tests hypotheses, rules out causes one by one, and delivers a plain-English report backed by the supporting evidence.

## Why this exists

I lived this experience at Kraft Heinz. A real bottleneck in CPG demand forecasting is investigating the source of anomalies — varied data sources, many potential causes, and significant planner time spent per flag. An agent that autonomously works through each candidate cause, rules it out, and reports its findings speeds the investigation up and gives planners their hours back.

## Roadmap

- [ ] Week 0 — Foundation: repo scaffolding, tooling, CI _(in progress)_
- [ ] Week 1 — Data layer: M5 ingestion, anomaly injector, detector
- [ ] Week 2 — Agent core: LangGraph state machine, tools, evals
- [ ] Week 3 — UI & deployment: Streamlit viewer, observability
- [ ] Week 4 — Polish: validation notebook, write-up, launch

## License

MIT — see [LICENSE](./LICENSE).
