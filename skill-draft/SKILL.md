---
type: skill-draft
status: draft
source_package: "[[../../Generated-Packages/X Feedback Feature Factory/README|X Feedback Feature Factory]]"
tags: [skill-draft, hermes-agent, product-feedback]
---

# public-feedback-to-agent-feature skill draft

```markdown
---
name: public-feedback-to-agent-feature
description: Convert public X feedback into scoped Hermes Agent feature experiments, shipped proof, and follow-up posts.
---

# Public Feedback to Agent Feature

## Triggers
Use when a public X reply, quote, issue, or comment suggests a Hermes Agent feature, product workflow improvement, or agent capability demo.

## Steps
1. Capture the exact feedback as an x-intel note with source URL and quote.
2. Score the request: user value, public proof value, effort, risk, and fit with existing roadmap.
3. If the experiment should be isolated, create a blank profile: `hermes profile create <name> --no-skills`.
4. Add only the skills/tools required for the experiment.
5. Implement the smallest observable behavior change or prototype.
6. Link commit, artifact, and demo back to the source note.
7. Draft a concise public reply/update showing the shipped result.

## Pitfalls
- Do not overbuild from one viral comment; require a small, demonstrable slice.
- Do not mutate production agent config during a speculative experiment.
- Keep source, artifact, and commit linked so the flywheel is auditable.

## Verification
- Source note exists.
- Experiment profile or repo path is recorded.
- Commit/artifact link exists.
- Follow-up message has proof, not just a promise.
```
