# Capstone
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
│   └── rule_based_labeling.py
├── models/             # Trained model checkpoints
│   ├── yolov8_baseline.pt
│   └── crossvit_baseline.pth
├── notebooks/          # EDA and experimental notebooks
│   └── eda.ipynb
├── figures/            # Visualizations and diagrams
├── train_test/         # Training and testing scripts
│   ├── train_yolov8.py #Training,validation and results
│   └──train_crossvit.py#Training,validation and results
└── README.md           # Project documentation
