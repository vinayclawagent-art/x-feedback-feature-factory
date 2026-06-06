# Repo Readiness Experiment Proof Attachment

Source package: [[../../Generated-Packages/X Feedback Feature Factory/README|X Feedback Feature Factory]]
Loop: [[../../Improvement-Loops/X Feedback Feature Factory Loop|X Feedback Feature Factory Loop]]

Use this attachment when a dashboard seed row is ready for a blank-profile or repo-readiness experiment. It captures proof without pretending the experiment already happened.

## Candidate

- Dashboard seed row:
- Source X/intel note:
- Proposed repo or affected Hermes area:
- Operator:
- Date:

## Pre-flight checklist

- [ ] Candidate has a public/source-backed feedback note.
- [ ] Feature scope is small enough for one sandbox run or repo-readiness pass.
- [ ] Expected proof is defined before running commands.
- [ ] Failure mode is useful even if the feature is deferred.

## Repo-readiness experiment

| Check | Command / evidence slot | Result |
| --- | --- | --- |
| Local repo exists or can be cloned | `git -C <repo> status --short --branch` | |
| Source note/package linked | Obsidian wikilink + URL | |
| Minimal change path identified | file/path or issue link | |
| Test/verification command chosen | command or manual check | |
| Follow-up proof target chosen | X reply/post, package changelog, PR, or commit link | |

## Blank-profile experiment

```bash
hermes profile create <feedback-slug> --no-skills
hermes profile use <feedback-slug>
# Reproduce the feedback in the smallest possible setting.
# Capture command output, screenshot path, or failure note below.
hermes profile use default
```

## Evidence block

- Commands run:
- Key output or screenshot path:
- Commit / PR / package link:
- Decision: `ship` / `iterate` / `defer`
- Proof-post draft link:

## Copyable package changelog line

```markdown
- YYYY-MM-DD: Ran repo-readiness / blank-profile proof for [[<seed row>]]; decision: <ship|iterate|defer>; evidence: <link>.
```

## Next action after completion

Attach the filled evidence block to [[Feedback Dashboard Seed Rows]], update the package changelog, then decide whether the skill draft has enough live proof to promote.
