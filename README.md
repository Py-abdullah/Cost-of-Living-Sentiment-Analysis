# Cost of Living Sentiment Analysis with RoBERTa

An NLP and Deep Learning project for analyzing sentiment in cost-of-living related tweets using **VADER Sentiment Analysis** and a fine-tuned **RoBERTa Transformer** model.

The project covers the complete workflow from data collection and preprocessing to sentiment labeling, transformer fine-tuning, data augmentation, and model evaluation.

---

## 📌 Project Overview

The goal of this project is to classify cost-of-living related tweets into three sentiment categories:

* 🔴 **Negative**
* ⚪ **Neutral**
* 🟢 **Positive**

VADER is initially used to generate sentiment labels, which are then used to train a transformer-based sentiment classification model using **RoBERTa**.

An additional data augmentation stage is performed using emojis and slang variations to improve model performance.

---

## 🚀 Key Features

* Tweet data collection using KaggleHub
* Text preprocessing and cleaning
* UK-related tweet filtering
* VADER-based sentiment labeling
* Exploratory data analysis and visualization
* Word cloud generation
* RoBERTa tokenization
* Transformer model fine-tuning
* Data augmentation using emojis and slang
* Model evaluation using multiple classification metrics
* Comparison of initial and augmented training results

---

## 🧠 Machine Learning Workflow

```text
Dataset
   ↓
Data Cleaning & Preprocessing
   ↓
UK Tweet Filtering
   ↓
VADER Sentiment Labeling
   ↓
Exploratory Data Analysis
   ↓
Train / Validation Split
   ↓
RoBERTa Tokenization
   ↓
RoBERTa Fine-Tuning
   ↓
Model Evaluation
   ↓
Data Augmentation
   ↓
Additional Fine-Tuning
   ↓
Final Evaluation
```

---

## 🛠️ Technologies & Libraries

| Technology                | Purpose                        |
| ------------------------- | ------------------------------ |
| Python                    | Core programming language      |
| Google Colab              | Development environment        |
| Pandas                    | Data manipulation              |
| NumPy                     | Numerical computing            |
| Matplotlib                | Data visualization             |
| Seaborn                   | Statistical visualization      |
| VADER                     | Initial sentiment labeling     |
| Hugging Face Transformers | Transformer-based NLP          |
| RoBERTa                   | Sentiment classification model |
| PyTorch                   | Deep learning framework        |
| Scikit-learn              | Data splitting and evaluation  |
| WordCloud                 | Text visualization             |
| KaggleHub                 | Dataset downloading            |

---

## 🤖 Model

The main model used in this project is:

**RoBERTa (`roberta-base`)**

The pretrained RoBERTa model is fine-tuned for **three-class sentiment classification**.

### Sentiment Classes

| Class    | Label |
| -------- | ----: |
| Negative |     0 |
| Neutral  |     1 |
| Positive |     2 |

---

## 📊 Results

### Initial RoBERTa Fine-Tuning

| Metric    |  Score |
| --------- | -----: |
| Accuracy  | 87.95% |
| Precision | 87.97% |
| Recall    | 87.95% |
| F1-Score  | 87.56% |

### RoBERTa with Data Augmentation

| Metric    |  Score |
| --------- | -----: |
| Accuracy  | 91.41% |
| Precision | 91.41% |
| Recall    | 91.41% |
| F1-Score  | 91.29% |

The augmented training experiment produced higher validation metrics than the initial fine-tuning experiment.

---

## 📂 Dataset

The project uses a **Cost of Living** tweet dataset downloaded through KaggleHub.

The notebook automatically downloads the dataset using:

```python
kagglehub.dataset_download("tleonel/cost-of-living")
```

The dataset contains tweets that are processed and filtered for the project's sentiment analysis task.

## 📁 Repository Structure

```text
Cost-of-Living-Sentiment-Analysis/
│
├── Cost_of_Living_With_Transformers.ipynb
├── README.md
└── requirements.txt
```

---

## 🎯 Learning Outcomes

Through this project, I worked with:

* Natural Language Processing (NLP)
* Sentiment Analysis
* Text preprocessing
* Exploratory Data Analysis (EDA)
* VADER sentiment analysis
* Hugging Face Transformers
* RoBERTa fine-tuning
* Data augmentation
* Model evaluation
* Python-based data analysis
* Deep Learning workflows

---

## 🔮 Future Improvements

Possible improvements include:

* Testing additional transformer models
* Using manually verified sentiment labels
* Performing hyperparameter optimization
* Adding confusion matrices and classification reports
* Evaluating the model on a separate external dataset
* Deploying the trained model as an API or web application

This project was developed as part of my practical learning and portfolio work in **Artificial Intelligence, Machine Learning, and Natural Language Processing**.
