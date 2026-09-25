# experiments/

One subfolder per experimental condition. Each will contain:

- `protocol.md`: exactly what was run, how many trials, and how it was measured
- processed results, kept small: summary tables and figures
- the analysis that produced them, or a pointer to it in `src/`

## Planned conditions

| Folder | Condition | What it isolates |
|---|---|---|
| `01-scripted-motion/` | Fixed, non-learned motion repeated N times | Mechanical + control repeatability |
| `02-servo-backlash/` | Bench test of a single STS3215 servo | Backlash specifically |
| `03-learned-policy/` | Trained policy repeated N times on the same task | The added, policy-induced variance |
| `04-intervention/` | Chosen once 01–03 show which source dominates | The improvement |

## Ground rule

Precision is never judged using the arm's own encoders or cameras. Every result here comes from an independent measurement.

## Large files

Raw recordings, datasets and model checkpoints are not stored in git. Datasets are published to the Hugging Face Hub and linked from the relevant `protocol.md`.
