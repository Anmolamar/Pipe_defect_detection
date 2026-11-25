AI-Based Pipe Defect Detection

Project Overview

This project uses a YOLO-based deep learning model to detect defects in pipe inspection images.

Detected Defect Classes

- Crack
- Hole
- Rupture
- Rust
- Void
- Corrosion

Model Details

- Model: YOLO11n
- Training epochs: 20
- Image size: 416 × 416
- Dataset: Combined pipe defect datasets

Trained Model

The complete trained project backup, including model weights and related files, is available here:

"Download FINAL_PIPE_PROJECT.zip" (https://drive.google.com/file/d/1SgJGG5CZuG_Yn5jRAnsoVlfIrb2d73hO/view?usp=sharing)

Repository Contents

- "best.pt" – Trained model weights
- "Pipe_Defect_Project_Results" – Training and evaluation results
- "README.md" – Project documentation

Usage

The trained model can be loaded using the Ultralytics YOLO library.

from ultralytics import YOLO

model = YOLO("best.pt")
results = model.predict("pipe_image.jpg", save=True)

Note

This project is a prototype for AI-based pipe defect detection. Prediction performance may vary depending on image quality and real-world conditions.
