# Repo Readiness Promotion Decision Card

Source package: [[../../Generated-Packages/X Feedback Feature Factory/README|X Feedback Feature Factory]]

Use this after filling [[Repo Readiness Experiment Proof Attachment]] for one real blank-profile or repo-readiness experiment. It turns evidence into a decision about whether a public-feedback seed should become a shipped Hermes improvement, a pilot-only change, or a held idea.

## Candidate row

- Feedback/source note:
- Source URL:
- Dashboard row:
- Experiment profile/repo:
- Run date:
- Operator:

## Evidence checklist

- [ ] The experiment includes exact commands or repo steps.
- [ ] The result includes a screenshot, terminal output, commit link, or other auditable proof.
- [ ] The result is connected back to the original public feedback.
- [ ] Regression or blast-radius risks are written down.
- [ ] Follow-up proof-post copy is drafted only if the change actually shipped.

## Decision options

Choose exactly one.

| Decision | Use when | Required next action |
| --- | --- | --- |
| `promote-to-feature` | The experiment reproduces the pain, validates the fix, and has low regression risk. | Open/ship the feature work and link commit/PR/proof. |
| `pilot-only` | The idea works for one repo/profile but is not general enough for default behavior. | Keep as a documented recipe or optional skill draft update. |
| `iterate` | The evidence is promising but missing commands, proof, or risk controls. | Add one scoped follow-up experiment before any public claim. |
| `hold` | The evidence is weak, duplicate, stale, or too risky. | Preserve the row but do not build or promote. |

Selected decision:

Rationale:

## Promotion guardrails

- Do not promote the skill draft until at least one real public-feedback seed has a filled proof attachment and this decision card.
- Do not publish a follow-up post unless there is shipped proof or a clearly labeled experiment result.
- If the decision is `pilot-only`, update the prototype README instead of changing Hermes defaults.

## Links to update after the real run

- Proof attachment:
- Dashboard seed row:
- Feature/PR/commit or recipe:
- Follow-up proof post draft:

## Outcome log

- Date:
- Decision:
- Files changed:
- Commit/repo link:
