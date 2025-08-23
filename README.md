# Project ZERO-G Vision
**Team:** Galactic 404
**Final mAP Score:** 0.865

## Description
This project uses a YOLOv8s model, trained on synthetic data from Duality's Falcon platform, to detect necessary equipment in a simulated space station environment. The methodical experimentation proved that a small model architecture was optimal, avoiding the overfitting observed in larger models.

## Environment Setup
1.  Ensure Anaconda is installed.
2.  Navigate to the `ENV_SETUP` subfolder (provided in the original dataset).
3.  Run `setup_env.bat` in an Anaconda Prompt to create the `EDU` environment.

## How to Reproduce Results
1.  Activate the environment: `conda activate EDU`
2.  Navigate to the main project folder.
3.  Run the prediction script: `python predict.py`
4.  The script will validate the included `best.pt` model and print the final results table, showing the 0.865 mAP score.
