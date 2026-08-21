## Sensor Fusion  and Ensemble Deep Learning for Wearable Sensor Data Analysis
**Human Activity Recognition (HAR) using Smart Belt, WISDM, and UCI Datasets**


## Highlights
- Deep learning models (CNN-LSTM, CNN-BiLSTM, CNN-GRU, CNN-BiGRU)
- Classical ensemble learners (Random Forest, Gradient Boosting)
- Stacked meta-learning architecture
- Evaluation on three datasets: Smart Belt, WISDM, and UCI HAR

---

## Models Included

| Model Notebook                          | Description                         |
|----------------------------------------|-------------------------------------|
| `CNN-GRU_Model_train_WISDM_500.ipynb`  | CNN with GRU                        |
| `CNN-LSTM_Hybrid_model_500.ipynb`      | CNN with LSTM                       |
| `CNN-BiGRU_Hybrid_model_500.ipynb`     | CNN with Bi-directional GRU         |
| `CNN-BiLSTM_Hybrid_model_500.ipynb`    | CNN with Bi-directional LSTM        |
| `1__Stacked_ensemble_hybrid_model.ipynb`| Final ensemble using RF and GBoost |

---
## Dataset Information

### 1. Smart Belt Dataset
- Collected from 12 participants using a custom belt with 3 IMU sensors (sampling rate: 100 Hz)
- Activities: Walking, walking upstairs/downstairs, sitting, standing, lying
- Annotated using [**NOVA**](https://github.com/hcmlab/nova)
- Dataset available in the [`Datasets/`](./Datasets/) folder (`smart_belt_dataset.csv`)  
  or [external link](https://alamedaproject.eu/)
- Oversampling applied to balance activity classes
  
### 2. WISDM v1.1
- Smartphone accelerometer data
- 6 activity classes: Walking, Jogging, Upstairs, Downstairs, Sitting, Standing
- Sampling rate: 20 Hz
- Used **undersampling** for class balancing
- WISDM Dataset Dataset link : https://www.cis.fordham.edu/wisdm/dataset.php
  
### 3. UCI HAR
- IMU data (accelerometer + gyroscope) from smartphones
- 6 activities: Walking, Upstairs, Downstairs, Sitting, Standing, Lying
- Sampling rate: 50 Hz
- Preprocessed and balanced → no resampling needed
- UCI HAR Dataset Dataset link: https://archive.ics.uci.edu/dataset/240/human+activity+recognition+using+smartphones

---

## How to Run

Clone the repository:

```bash
git clone https://github.com/AdaneNT/Ensemble-Deep-Learning.git
cd Ensemble-Deep-Learning
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Download the  dataset and place it in the project folder.

Launch Jupyter and run any model notebook:

```bash
jupyter notebook CNN-BiGRU_Hybrid_model_500.ipynb
```

For the ensemble model:

```bash
jupyter notebook 1__Stacked_ensemble_hybrid_model.ipynb
```

---

