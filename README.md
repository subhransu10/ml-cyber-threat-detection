# ML-Based Anomaly Detection for Web Traffic

🚨 A machine learning solution to detect anomalies in web traffic for the APPtake Hackathon 2025, leveraging unsupervised learning to spot hidden cyber threats.

## 🚀 Overview

This project was developed as part of the APPtake 1st Hackathon challenge, where the goal was to identify suspicious behaviors in real-world web traffic data using machine learning—without relying on labeled attack signatures.

## 📂 Dataset

Dataset: [Cybersecurity Suspicious Web Threat Interactions](https://www.kaggle.com/datasets/jancsg/cybersecurity-suspicious-web-threat-interactions)

Each record includes:
- Timestamps (`creation_time`, `end_time`)
- Source IP and country
- Destination domain/URL
- Bytes transferred (`bytes_in`, `bytes_out`)

## 🧠 ML Approach

We used unsupervised techniques including:
- Isolation Forest
- Clustering by `src_ip`, session behavior
- Custom time-based anomaly scoring

## 📊 Visualizations

- IP distribution heatmaps
- Anomaly timeline plots
- Feature-wise behavior scatter plots

## 🔧 Features Engineered

- Session duration
- Frequency of IP/domain access
- URL entropy & unusual structure detection
- Country-level outliers

## 💻 Tech Stack

- Python 3.x
- pandas, numpy, scikit-learn, matplotlib, seaborn
- Jupyter / Google Colab

## 🧪 How to Run

1. Clone the repo
2. Open the `notebooks/` folder
3. Run `main.ipynb` to explore EDA and model outputs

```bash
git clone https://github.com/yourusername/cyber-anomaly-detector.git
cd cyber-anomaly-detector
