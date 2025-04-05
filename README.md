# Capstone
<img width="469" alt="Screenshot 2025-03-31 at 22 56 57" src="https://github.com/user-attachments/assets/d315ae3e-ba6f-42b3-9408-a10e8e542045" />



Automated candle stick patttern recognition using YOLOv8 and CrossViT 
Author: Melvin Mathew

Affiliation: Rochester Institute of Technology, MS in Artificial Intelligence

Email: mmm5508@rit.edu

This project develops a hybrid self-improving system for automated candlestick pattern recognition in financial markets. It integrates rule-based labeling with deep learning models (YOLOv8 for object detection and CrossViT for classification) to detect and classify 12 key candlestick patterns from NIFTY50 stock data, enhancing trading decision-making.

candlestick_recognition/
├── data/                # Sample datasets (OHLC CSV and annotated images)
│   ├── raw/            # Raw NIFTY50 OHLC data and images data
│   └── annotated/      # Annotated images for training
├── scripts/            # Technical analysis labels for annotation
│   └── rule_based_labeling.ipynb
├── baselines/             # Baseline model 
│   ├── yolov8_baseline.ipynb
│   └── crossvit_baseline.ipynb
├── notebooks/          # EDA and experimental notebooks
│   └── eda.ipynb
├── figures/            # Visualizations and diagrams
├── code/         # Training and testing scripts
│   ├── yolov8.ipynb #Training,validation and results
│   └──crossvit.ipynb#Training,validation and results
└── README.md           # Project documentation

### Instructions to Run the Project

This section provides detailed steps to set up and run the project for automated candlestick pattern recognition using YOLOv8 and CrossViT. All code is provided in Jupyter notebooks (`.ipynb` files), and the required data is already included in the repository.

#### 1. Environment/Dependency Installation
To run the notebooks, you need a Python environment with the necessary dependencies. Follow these steps:

- **Clone the Repository**:
  ```bash
  git clone https://github.com/Melvinmm123/Capstone.git
  cd Capstone

Install Python Dependencies: The project requires Python 3.8 or higher. All required libraries are listed in requirements.txt. Install them using the following command:
pip install -r requirements.txt

- Data Preparation:
The dataset is already provided in the data/ directory, so no external downloading is required.

- Generate Annotations: The scripts/rule_based_labeling.ipynb notebook applies rule-based labeling to the raw NIFTY50 data to generate annotated images for training.
Run this notebook first:
In Jupyter, navigate to the scripts/ directory and open rule_based_labeling.ipynb.
Run all cells in the notebook. This will process the data/raw/nifty50 file, generate candlestick pattern labels

- Training/Testing Demo Scripts
The project includes notebooks for exploratory data analysis (EDA), baseline models, and the main training/testing pipeline. Run them in the following order to replicate the results:

- Exploratory Data Analysis: To explore the dataset and visualize candlestick patterns:
In Jupyter, navigate to notebooks/ and open eda.ipynb.
Run all cells to generate visualizations of the data 

- Baseline Models: To evaluate the baseline performance of YOLOv8 and CrossViT:
Navigate to baselines/ and open yolov8_baseline.ipynb.
Run all cells to train and test the YOLOv8 baseline model on the annotated images.
Open crossvit_baseline.ipynb.
Run all cells to train and test the CrossViT baseline model for classification.

- Main Training and Testing: The core implementation is in the code/ directory:
-YOLOv8 Training and Validation:
Navigate to code/ and open yolov8.ipynb.
Run all cells to train YOLOv8 on the annotated images, validate the model, and generate predictions.

-CrossViT Training and Validation:
Open code/crossvit.ipynb.
Run all cells to train CrossViT for classifying candlestick patterns, validate the model, and generate results.

