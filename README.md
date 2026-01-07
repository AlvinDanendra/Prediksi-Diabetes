# Diabetes Prediction using Machine Learning

Project ini bertujuan untuk memprediksi apakah seseorang terdiagnosis diabetes berdasarkan data kesehatan menggunakan pendekatan machine learning classification.

## Deskripsi Project
Pada project ini dilakukan:
- Exploratory Data Analysis (EDA)
- Preprocessing data (scaling menggunakan StandardScaler)
- Perbandingan beberapa model machine learning
- Evaluasi model menggunakan beberapa metrik
- Prediksi data testing menggunakan model terbaik

Karena distribusi kelas tidak seimbang, evaluasi tidak hanya berfokus pada accuracy, tetapi juga metrik lain yang lebih representatif.

## Dataset
Dataset berisi data kesehatan individu dengan target:
- `diagnosed_diabetes`
  - 1 : Terdiagnosis diabetes
  - 0 : Tidak terdiagnosis diabetes

Distribusi kelas:
- Diabetes : ~62%
- Non-diabetes : ~38%

## Model yang Digunakan
Beberapa model yang diuji menggunakan cross-validation:
- Logistic Regression
- Random Forest Classifier
- Support Vector Classifier (SVC)

## Evaluasi Model
Model dievaluasi menggunakan:
- Accuracy
- Recall
- F1 Score

Hasil menunjukkan bahwa seluruh model memiliki accuracy yang relatif serupa (~0.66).  
Hal ini mengindikasikan bahwa performa model dibatasi oleh kualitas dan informasi fitur yang tersedia.

Oleh karena itu, pemilihan model difokuskan pada kombinasi metrik (Accuracy, Recall, dan F1 Score), bukan accuracy saja.

## Model Terbaik
Model terbaik dipilih berdasarkan skor gabungan dari:
- Accuracy
- Recall
- F1 Score

Berdasarkan evaluasi tersebut, model dengan performa paling stabil digunakan untuk melakukan prediksi pada data testing.

## Prediksi Data Testing
Model terbaik dilatih ulang menggunakan seluruh data training, kemudian digunakan untuk memprediksi data testing.  
Hasil prediksi disimpan dalam format DataFrame untuk keperluan analisis atau submission.

## Tools & Library
- Python
- Pandas
- NumPy
- Scikit-learn
- Jupyter Notebook

## Catatan
Performa model dibatasi oleh ketidakseimbangan kelas dan keterbatasan fitur.  
Peningkatan performa di masa depan dapat dilakukan melalui feature engineering atau penambahan data yang lebih informatif.

## Author
Alvin Danendra
