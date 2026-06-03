# Blank-Profile Experiment Template

Source loop: [[../../Improvement-Loops/X Feedback Feature Factory Loop|X Feedback Feature Factory Loop]]

Use this when an X comment suggests a Hermes behavior change that should be tested without inherited skills, memories, or plugin assumptions.

## 1. Feedback input

| Field | Value |
|---|---|
| X source URL |  |
| Author / handle |  |
| Raw feedback |  |
| Interpreted request |  |
| Artifact package | [[../../Generated-Packages/X Feedback Feature Factory/README|X Feedback Feature Factory]] |

## 2. Score before building

| Dimension | 1 | 3 | 5 | Score |
|---|---|---|---|---|
| Public proof | Vague complaint | Clear request | Strong public example + reply path |  |
| User impact | Nice-to-have | Saves repeated manual work | Unlocks a new agent workflow |  |
| Implementation effort | Multi-week | 1-2 days | Same-day patch/test |  |
| Regression risk | Core behavior risk | Isolated command/setting | Profile-scoped or opt-in |  |
| Demo clarity | Hard to show | Screenshotable | One command + before/after proof |  |

Decision rule: build when average score is **3.8+** and regression risk is not the highest-scoring concern.

## 3. Sandbox profile

```bash
# Pick a short, disposable name tied to the feedback item.
hermes profile create x-feedback-<slug> --no-skills

# Run the smallest reproduction in that profile before changing defaults.
hermes --profile x-feedback-<slug>
```

## 4. Experiment checklist

- [ ] Reproduce the current behavior in the blank profile.
- [ ] Write the expected behavior in one sentence.
- [ ] Implement the smallest profile-scoped or opt-in change.
- [ ] Re-run the reproduction and capture terminal/browser proof.
- [ ] Link commits, screenshots, or notes back to the X source.
- [ ] Draft a short public reply: what changed, how to try it, where proof lives.

## 5. Follow-up proof post format

```text
Shipped a small Hermes improvement from this feedback:

Before: <one-line pain>
After: <one-line capability>
Try: <command or link>
Proof: <screenshot/commit/demo>

Thanks for the push — this is now in the agent workflow.
```

## Notes

Keep these experiments intentionally small. If the fix needs a broad architecture change, promote it into a normal product backlog item instead of forcing it through the public-feedback fast lane.
