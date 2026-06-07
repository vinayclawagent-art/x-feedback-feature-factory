# X Feedback Feature Factory Prototype

Source package: [[../../Generated-Packages/X Feedback Feature Factory/README|X Feedback Feature Factory]]

Open `index.html` in a browser.

Demonstrates a public-feedback-to-agent-feature triage board: capture, classify, experiment in blank-slate profile, ship, publish proof.

## Added templates

- [[Feature-Intake Scoring Template]] — score public proof, impact, effort, confidence, and regression risk before building.
- [[Blank-Profile Experiment Template]] — run the smallest reproduction with `hermes profile create <slug> --no-skills`, capture proof, and draft the follow-up post.
- [[Weekly Feedback Dashboard Query]] — weekly dashboard spec for recent feedback candidates, shipped proof, blank-profile tests, and proof-post gaps.
- [[Feedback Dashboard Seed Rows]] — first concrete dashboard pass with three recent X-intel candidates, scores, experiment links, and next actions.
- [[Repo Readiness Experiment Proof Attachment]] — fillable evidence block for the next blank-profile or repo-readiness test; keeps the loop concrete without inventing proof before a real run.
- [[Repo Readiness Promotion Decision Card]] — fillable promote-to-feature / pilot-only / iterate / hold card that turns the next real proof attachment into a clear product decision.

## Next iteration

Fill [[Repo Readiness Experiment Proof Attachment]] and [[Repo Readiness Promotion Decision Card]] for the highest-scoring seed row, then promote only rows with concrete sandbox commands, commit links, risk notes, and proof replies into `_Dashboards/Artifact-Factory.md`.
