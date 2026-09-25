# src/

Code written for this project. It is empty for now. The first code will be measurement and analysis scripts, once the arm is assembled and calibrated.

## What's *not* here

LeRobot itself. It is an external dependency (Hugging Face's robotics framework), installed separately rather than copied into this repo. The setup used here, as of 2026-09 (check LeRobot's own install docs for current steps):

```bash
conda create -n lerobot python=3.12
conda activate lerobot
conda install ffmpeg -c conda-forge
git clone https://github.com/huggingface/lerobot.git
cd lerobot
pip install -e ".[feetech]"
```

Current LeRobot requires Python ≥ 3.12. Some older third-party SO-101 guides still say 3.10, and that install fails.
