# ZERO-G VISION
### Object Detection for Astronaut Safety using Synthetic Data
*Submission for the Hackground India 2k25 Hackathon (Duality AI Track) by Team Galactic 404.*

## 🚀 Project Overview
Project ZERO-G VISION is a high-performance object detection model designed to enhance crew safety on space stations. The model is trained exclusively on synthetic data from Duality AI's Falcon platform to identify critical equipment: **Toolboxes**, **Oxygen Tanks**, and **Fire Extinguishers**. This project demonstrates a complete workflow from data analysis and model training to methodical experimentation and final evaluation.

## 📊 Key Features & Final Result
* **High Accuracy:** Achieved a final **mAP@0.5 score of 0.865** on the test dataset.
* **Optimized Model:** Proven through experimentation that the **YOLOv8s** architecture provides the optimal balance of speed and accuracy for this task.
* **3 Object Classes:** Successfully detects all three critical object classes in varied and challenging simulated environments.

## 🔬 Our Experimental Journey
Our core methodology was data-driven experimentation. We first established a strong baseline by training a `yolov8s` model for 50 epochs, which achieved an excellent **0.865 mAP**. We then hypothesized that a larger `yolov8m` model could yield even better results.

However, a full training cycle revealed that the larger model began to overfit the dataset, resulting in a lower score of **0.834 mAP**. This crucial insight allowed us to definitively select the `yolov8s` model as the champion for our final submission.

## 🛠️ Tech Stack
* **AI Framework:** Python, PyTorch, Ultralytics YOLOv8
* **Environment:** Anaconda
* **Dataset:** Duality AI Falcon (Synthetic Data)
* **Hardware:** NVIDIA GeForce RTX 2050

## ▶️ How to Reproduce Results

#### Environment Setup
1.  Ensure Anaconda is installed.
2.  Navigate to the `ENV_SETUP` subfolder (provided in the original dataset).
3.  Run `setup_env.bat` in an Anaconda Prompt to create and set up the `EDU` environment.

#### Run Prediction
1.  Activate the environment: `conda activate EDU`
2.  Navigate to the main project folder.
3.  Run the prediction script: `python predict.py`
4.  The script will validate the included `best.pt` model and print the final results table, showing the 0.865 mAP score.

## 👩‍🚀 Team Members – Team Galactic 404

- **Saurish Sagar** – [GitHub](https://github.com/SaurishS)
- **Anu Singh** – [GitHub](https://github.com/anu-singh2507)
