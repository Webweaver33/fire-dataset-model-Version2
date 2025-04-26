# fire-dataset-model-Version2
# Forest Fire and Animal Detection Using Deep Learning and Hypergraph Fusion

## Overview
This project focuses on early detection of **forest fires** and **wildlife presence** using advanced **deep learning models**, followed by intelligent fusion through a **hypergraph-based model** to improve decision-making in forest monitoring systems.

## Key Components
- **Fire Detection**:  
  - Model: **VGG19** (Convolutional Neural Network)  
  - Trained to detect signs of forest fires from image data.
  
- **Animal Detection**:  
  - Model: **YOLOv5** (You Only Look Once, Version 5)  
  - Trained for real-time wildlife detection in forest environments.

- **Fusion Model**:  
  - Technique: **Hypergraph-based Fusion**  
  - Combines the outputs of fire and animal detection models to produce a more comprehensive environmental assessment.

## Project Structure
```
/forest-fire-animal-detection
│
├── data/                 # Datasets for fire and animal detection
├── models/               # Trained VGG19 and YOLOv5 models
├── fusion/               # Hypergraph fusion code
├── notebooks/            # Jupyter notebooks for experiments and training
├── utils/                # Helper scripts (preprocessing, evaluation metrics, etc.)
├── results/              # Detection results and fusion outputs
├── README.md             # Project description
└── requirements.txt      # List of Python dependencies
```

## Data Requirements
- **Fire Detection Dataset**:  
  - Forest fire image datasets (with augmented data for better robustness)
- **Animal Detection Dataset**:  
  - Wildlife image datasets suited for YOLO training
- **Preprocessing**:  
  - Data cleaning, augmentation, normalization, and annotation preparation

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/Webweaver33/fire-dataset-model-Version2.git
   cd fire-dataset-model-Version2
   ```

2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Download and place datasets in the `/data` directory.

## Usage
1. Train or load pretrained models:
   - Fire detection (VGG19):  
     ```bash
     python train_fire_detection.py
     ```
   - Animal detection (YOLOv5):  
     ```bash
     python train_animal_detection.py
     ```

2. Run inference on new data:
   ```bash
   python detect_fire.py
   python detect_animals.py
   ```

3. Perform hypergraph-based fusion:
   ```bash
   python hypergraph_fusion.py
   ```

4. View results in the `/results` folder.

## Features
- Accurate fire and animal detection using state-of-the-art deep learning models
- Advanced fusion strategy using hypergraph modeling for multi-modal decision making
- Scalable and modular project structure
- Extensive data augmentation and preprocessing

## Limitations
- No alert system is currently integrated.
- Requires high-quality datasets for optimal performance.

## Future Work
- Integration with real-time sensor data (e.g., IoT devices, satellite images)
- Development of an alerting and notification system
- Optimization of hypergraph models for faster processing

## Contributor
- **K. Mohan Krishna**
