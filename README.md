# 🏥 Medical Transcriptions NLP Preprocessing

This project implements a complete Natural Language Processing (NLP) pipeline to clean, augment, and process medical transcription data. The goal is to prepare raw medical text for classification or analysis tasks.

## 🚀 Key Features
* **Data Cleaning:** Handling missing values, removing duplicates (removed 2600+ duplicates).
* **Advanced Preprocessing:**
    * De-emojising & HTML tag removal.
    * Text normalization & Special character removal.
    * Stopword removal (customized to keep medical terms like 'no', 'not').
    * Lemmatization & OOV (Out of Vocabulary) handling.
* **Data Augmentation:** Oversampling minority medical specialty classes to balance the dataset.
* **Feature Extraction:** Generating TF-IDF vectors (Top 5000 features).

## 🛠️ Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, NLTK, Scikit-learn, Imbalanced-learn

## 📊 Pipeline Steps
1.  **Duplicate Removal:** Reduced dataset from ~5000 to 2358 unique rows.
2.  **Missing Value Handling:** Filled null values in description and specialty columns.
3.  **Text Preprocessing:** Applied tokenization and normalization.
4.  **Class Balancing:** Identified minority classes (<100 samples) and applied augmentation.
5.  **Vectorization:** Converted processed text into TF-IDF matrix.

## 📂 How to Use
1.  Clone the repository.
2.  Install dependencies: `pip install pandas nltk scikit-learn imbalanced-learn`
3.  Run the `Medical_Text_Preprocessing.ipynb` notebook.
