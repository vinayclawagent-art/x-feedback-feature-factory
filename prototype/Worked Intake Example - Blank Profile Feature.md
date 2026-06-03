# Worked Intake Example: Blank Profile Feature

Source package: [[../../Generated-Packages/X Feedback Feature Factory/README|X Feedback Feature Factory]]
Source note: [[../../../Tools/X Feedback as a Feature Factory for Hermes Agents|X Feedback as a Feature Factory for Hermes Agents]]
Source URL: https://x.com/Saboo_Shubham_/status/2052601648074383576
Quoted feature URL: https://x.com/Teknium/status/2052351650279645590
Created: 2026-06-03

## Intake

- **Author:** @Saboo_Shubham_ / Shubham Saboo
- **Exact ask / quote:** “Hermes Agent team (@NousResearch) is going from X comments to fully working features in hours.”
- **Feature proof:** `hermes profile create <name> --no-skills` creates a fresh agent profile with no built-in skills.
- **Existing Hermes feature area:** profiles, skills, agent configuration, public feedback loop.

## Scores (1-5)

| Dimension | Score | Notes |
|---|---:|---|
| User value | 5 | Blank profiles remove inherited-skill noise and make focused agent experiments easier. |
| Public proof value | 5 | The shipped command is concrete, tweetable, and directly validates the “comments → feature” loop. |
| Effort | 4 | Small CLI/config surface if profile plumbing already exists; docs/tests still required. |
| Risk | 4 | Safe if implemented as opt-in profile creation and never mutates the default profile. |
| Roadmap fit | 5 | Strengthens Hermes as an agent-building platform and supports Vinay’s specialized-agent workflow. |

## Decision

- **Total:** 23 / 25
- **Decision:** build now / document as canonical exemplar
- **Sandbox profile name:** `feedback-blank-profile-demo`
- **Command:** `hermes profile create feedback-blank-profile-demo --no-skills`

## Smallest shippable slice

- **Observable behavior change:** user can create a profile that starts without the default skill set.
- **Test/verification:** run profile creation, inspect the profile skills directory/config, confirm no built-in skills are attached by default.
- **Artifact/commit link:** this worked example plus the follow-up proof-post template.
- **Follow-up proof message:** “A public X comment turned into an opt-in blank-profile command: here’s the command, the empty-skill verification, and how to use it for focused agent experiments.”

## Reuse rule

For the next feedback-derived feature, clone this worked example first and change only the source, scores, and smallest shippable slice. If the total score is below 18, hold it unless Vinay explicitly promotes it.
