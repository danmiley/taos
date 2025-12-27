# Idea-Template: Universal Subheadings and Variations

Purpose: provide a reusable spine for any concept-focused repo (e.g., “accelerating AI adoption in the enterprise”).

## Core Subheadings (works across topics)
1) Executive Snapshot  
- One-liner; primary goal; who benefits; success in one sentence.

2) Why Now / Context  
- Market/field drivers, constraints, inflection points; prior attempts and why they stalled.

3) Problem Definition & Boundaries  
- Pain points; in-scope vs out-of-scope; assumptions; falsifiability tests.

4) Stakeholders & Audiences  
- Personas, incentives, blockers; internal vs external; human stories.

5) Use Cases / Journeys  
- Top scenarios; before/after flows; edge cases; moments that fail today.

6) Evidence Base & Signals  
- Facts, metrics, precedents, benchmarks; contrary data; open data gaps.

7) Option Set / Approaches  
- Baseline, stretch, no-change, and “do nothing” options; design principles; trade-offs.

8) Architecture / Operating Model  
- If technical: system diagram, data flows, integration points, safety rails.  
- If programmatic: roles, processes, governance cadence, decision rights.

9) Implementation Plan & Milestones  
- Phases, dependencies, owners, risks per phase; minimal viable slice first.

10) Change Management & Adoption  
- Comms plan, training, incentives, policy updates, feedback loops; adoption risks.

11) Metrics & Success Criteria  
- Leading/lagging metrics; narrative “how we’ll know it’s working”; failure thresholds.

12) Governance, Risk, and Ethics  
- Failure modes; safety, compliance, privacy; kill-switch rules.

13) Economics & Resourcing  
- Costs (build/run/change), funding model, ROI ranges, sensitivity analysis.

14) Open Questions & Decision Log  
- Unresolved items with owners; decisions with date/rationale; reversibility notes.

15) Sources & Research Backlog  
- Citations, interviews, datasets; what to find next; confidence levels.

16) Narrative Highlights  
- Short list of the most compelling stories/findings (optionally note surprises/turning points).

## Swap-Ins and Extensions
- **Product/Service flavor:** Customer segments; value proposition; competitive landscape; pricing/packaging; distribution.  
- **Policy flavor:** Legal context; stakeholder map; enforcement/measurement; sunset/renewal criteria.  
- **R&D flavor:** Hypotheses; experiment design; instrumentation; replication plan; peer review path.  
- **Creative/media flavor:** Audience promise; mood/tone; formats; release cadence; IP/licensing; visual/audio palette.  
- **Data/ML flavor:** Data inventory; quality risks; model card; evaluation protocols; alignment/guardrails; drift/monitoring; incident response.

## Example Layout for “Accelerating AI Transformation in the Enterprise”
- Executive Snapshot: What “good” looks like in 12 months; top KPI.  
- Why Now: Competitive pressures, budget cycle window, regulatory headwinds.  
- Problem Definition: Where pilots stall (procurement, data access, trust).  
- Stakeholders: IT, security, legal, data owners, business units, frontline users.  
- Use Cases: 5 prioritized journeys (e.g., contract review, support copilots) with before/after.  
- Evidence Base: Productivity benchmarks; failure post-mortems; reference implementations.  
- Option Set: Central platform vs BU-led vs hybrid; “no-change” baseline for contrast.  
- Architecture: Data ingress/egress, PII handling, red-teaming loop, human-in-the-loop points.  
- Change Management: Training by persona; comms drumbeat; incentive alignment; success stories.  
- Metrics: Activation, weekly active use, task-level quality, time-to-value, risk incidents.  
- Governance/Risk: Model risk taxonomy; approval gates; rollback triggers; audit trail.  
- Economics: Build/run cost bands; vendor/infra sensitivity; value-at-risk if delayed.  
- Open Questions: Data residency, IP indemnity, human review staffing, citation policy.

## Case-Style Option (Harvard-like framing, optional)
- Situation: What’s happening now and why it matters.  
- Complication: The tension, constraint, or blocker.  
- Options: Realistic paths with pros/cons and required enablers.  
- Recommendation: Clear choice plus rationale.  
- Implementation: Phasing, owners, milestones, risks, contingencies.  
- Exhibits: Data tables, timelines, org charts, financials.

## Lightweight Prompt to Generate a New Topic Repo from This Spine
“Instantiate an `idea-template` for [TOPIC]. Use the core subheadings. Add swap-ins for [flavor]. Produce initial drafts for: Executive Snapshot, Why Now, Problem Definition, Stakeholders, Top 3 Use Cases, Evidence Base, Option Set, Metrics, Governance/Risk, and Open Questions. Keep sections concise but specific enough to act.”

