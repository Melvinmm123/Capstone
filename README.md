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
├── train_test/         # Training and testing scripts
│   ├── train_yolov8.ipynb #Training,validation and results
│   └──train_crossvit.ipynb#Training,validation and results
└── README.md           # Project documentation


