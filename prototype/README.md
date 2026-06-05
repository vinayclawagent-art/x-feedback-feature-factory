# X Feedback Feature Factory Prototype

Source package: [[../../Generated-Packages/X Feedback Feature Factory/README|X Feedback Feature Factory]]

Open `index.html` in a browser.

Demonstrates a public-feedback-to-agent-feature triage board: capture, classify, experiment in blank-slate profile, ship, publish proof.

## Added templates

- [[Feature-Intake Scoring Template]] — score public proof, impact, effort, confidence, and regression risk before building.
- [[Blank-Profile Experiment Template]] — run the smallest reproduction with `hermes profile create <slug> --no-skills`, capture proof, and draft the follow-up post.
- [[Weekly Feedback Dashboard Query]] — weekly dashboard spec for recent feedback candidates, shipped proof, blank-profile tests, and proof-post gaps.
- [[Feedback Dashboard Seed Rows]] — first concrete dashboard pass with three recent X-intel candidates, scores, experiment links, and next actions.

## Next iteration

Run the weekly dashboard query on the next seven days of X feedback, then promote only rows with concrete sandbox commands, commit links, and proof replies into `_Dashboards/Artifact-Factory.md`.
