# Weekly Feedback Dashboard Query

Package: [[../../Generated-Packages/X Feedback Feature Factory/README|X Feedback Feature Factory]]

Use this query/spec once per week to turn scattered public X feedback into a small, auditable Hermes improvement dashboard.

## Dashboard sections

| Section | Query / filter | Done condition |
|---|---|---|
| New feedback candidates | Notes tagged `x-intel` or `feedback-loop` from the last 7 days with a source URL and explicit user pain. | Up to 5 rows scored with the intake template. |
| Shipped from feedback | Package/prototype notes whose change log mentions public feedback, a commit, or a proof post. | Each row has source note, shipped artifact, proof link, and follow-up status. |
| Needs blank-profile test | Items with high public proof but unclear regression risk. | Each row links to a blank-profile experiment note or is marked `defer`. |
| Proof-post backlog | Shipped changes without a before/after screenshot, reproduction note, or source-thread reply. | Each row has a next proof action and owner. |

## Copyable dashboard row

```markdown
| Source | Pain | Score | Experiment | Shipped proof | Next action |
|---|---:|---:|---|---|---|
| [[Source Note]] | <one-line user pain> | <0-25> | [[Blank Profile Experiment]] | <commit/proof-post URL> | <ship / test / defer> |
```

## Weekly operating rule

Only promote a feedback item into a build artifact when it has:

1. A public source URL or reproducible user quote.
2. A score of **18/25+** on [[Feature-Intake Scoring Template]].
3. A smallest-safe sandbox plan using [[Blank-Profile Experiment Template]].
4. A visible proof path using [[Follow-Up Proof Post Template]].

## Next use

Run this query against the next seven days of X feedback notes, add the top 3 rows to `_Dashboards/Artifact-Factory.md` or a package-specific dashboard, and link any shipped changes back to the source note.
