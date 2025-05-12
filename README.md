# ML-Based Anomaly Detection for Web Traffic

🚨 A machine learning solution to detect anomalies in web traffic for the APPtake Hackathon 2025, leveraging unsupervised learning to spot hidden cyber threats.

## 🤝 Collaborators
### <img src="https://user-images.githubusercontent.com/62358773/158238810-c5dcb486-ba24-4b35-87de-39a54e88f36b.png" width="5%" height="5%"> [Subhransu Sourav Priyadarshan](https://github.com/subhransu10) <img src="https://user-images.githubusercontent.com/62358773/158238810-c5dcb486-ba24-4b35-87de-39a54e88f36b.png" width="5%" height="5%"> [Luca Martini](https://github.com/luke9705)

## 🚀 Overview

This project was developed as part of the APPtake 1st Hackathon challenge, where the goal was to identify suspicious behaviors in real-world web traffic data using machine learning without relying on labeled attack signatures.

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
- Multiple contamination levels were tested ('auto', '0.01' to '0.3')
- StandardScaler normalization on numerical features before fitting
- One-hot encoding for categorical features ('src_ip_country_code', 'src_ip')
- PCA analysis for key features extraction from the dataset
- DBSCAN to categorize the anomalies

## 📊 Visualizations

- Source country codes by request count
- Bytes in vs Bytes out by country (sampled)
- Top countries by the number of anomalies
- DBSCAN of outlier group clusters in PCA space
- Feature-wise behavior scatter plots
- t-SNE visualization of the comparision of different methods (isolation forest, DBSCAN and integrated method)

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
2. Run `apptake.ipynb` to explore EDA and model outputs
3. Also you can also access the '.csv' files

```bash
git clone https://github.com/subhransu10/ml-cyber-threat-detection.git

