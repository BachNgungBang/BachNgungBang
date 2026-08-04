# Workflows

GitHub Actions workflows for this profile belong in this directory.

Use workflows only for repeatable automation, such as scheduled profile-stat generation or validation. Pin third-party actions to immutable commit SHAs, use least-privilege permissions, and avoid creating commits when generated output has not changed.

## Included automation

| Workflow | Output | Update schedule |
|---|---|---|
| `contribution-snake.yml` | Purple/blue contribution snake in the `output` branch. | Daily + manual run |
| `profile-summary-cards.yml` | `profile-summary-card-output/` SVG cards on `main`. | Every 12 hours + manual run |
| `readme-metrics.yml` | `assets/generated/readme-metrics.svg` on `main`. | Daily + manual run |

`readme-metrics.yml` needs a personal access token in the `METRICS_TOKEN` repository secret. The standard GitHub Stats, activity graph, streak, trophy, and visitor widgets in `README.md` are remote dynamic images: they refresh at render time, so they do not need a scheduled workflow or repository write access.
