# Music Recommendation System Using Convolutional Neural Networks

## Overview

This project presents a Music Recommendation System developed using Convolutional Neural Networks (CNNs) and audio signal processing techniques. The system analyzes music tracks, learns audio patterns from spectrogram representations, classifies songs into genres, and recommends similar songs based on learned feature embeddings.

The project was developed as part of an undergraduate Neural Networks course project and demonstrates the application of deep learning techniques in music information retrieval and recommendation systems.

---

## Objectives

* Develop a CNN-based model for music genre classification.
* Extract meaningful audio features from music tracks.
* Generate song embeddings using a trained neural network.
* Recommend similar songs based on audio feature similarity.
* Demonstrate the use of deep learning in music recommendation applications.

---

## Dataset

The project uses the GTZAN Music Genre Classification Dataset.

Dataset Characteristics:

* 1000 audio tracks
* 10 music genres
* 100 tracks per genre
* Each audio file is approximately 30 seconds long

Genres Included:

* Blues
* Classical
* Country
* Disco
* Hip-Hop
* Jazz
* Metal
* Pop
* Reggae
* Rock

Dataset Source:

https://www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification

---

## Project Workflow

Audio File

↓

Audio Preprocessing

↓

Mel Spectrogram Generation

↓

CNN Feature Learning

↓

Genre Classification

↓

Feature Embedding Extraction

↓

Similarity Calculation

↓

Music Recommendation

---

## Technologies Used

### Programming Language

* Python

### Libraries and Frameworks

* TensorFlow
* Keras
* Librosa
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* Joblib

### Development Environment

* Google Colab
* Jupyter Notebook

---

## Feature Extraction

The audio files are converted into Mel Spectrogram representations before being fed into the neural network.

Extracted audio representations include:

* Waveforms
* Mel Spectrograms
* MFCC (Mel Frequency Cepstral Coefficients)

These representations allow the CNN to learn frequency and temporal characteristics of music tracks effectively.

---

## CNN Architecture

The model consists of:

* Convolutional Layers
* Batch Normalization Layers
* Max Pooling Layers
* Dropout Layers
* Dense Embedding Layer
* Softmax Output Layer

The embedding layer generates compact feature representations that are used for music similarity search and recommendation.

---

## Training and Evaluation

The model is trained using:

* Adam Optimizer
* Categorical Cross-Entropy Loss
* Early Stopping
* Learning Rate Reduction

Evaluation metrics include:

* Accuracy
* Loss
* Classification Report
* Confusion Matrix

---

## Recommendation System

After training, feature embeddings are extracted from the CNN.

Recommendations are generated using:

1. Genre Prediction
2. Feature Embedding Extraction
3. Cosine Similarity Calculation
4. Retrieval of Most Similar Songs

This approach enables content-based music recommendation using learned audio characteristics.

---

## Project Structure

```text
music-recommendation-system-cnn/
│
├── data/
│   ├── genres_original/
│
├── model/
│   ├── music_genre_cnn_final.keras
│
├── artifacts/
│   ├── music_reco_artifacts.joblib
│
├── notebooks/
│   ├── Music_Recommendation_System.ipynb
│
├── results/
│   ├── confusion_matrix.png
│   ├── training_curves.png
│
├── README.md
└── requirements.txt
```

## Sample Output

Input Song:

```text
metal.00000.wav
```

Predicted Genre:

```text
Metal
```

Recommended Songs:

```text
metal.00038.wav
metal.00098.wav
metal.00088.wav
metal.00070.wav
metal.00087.wav
```

---

## Future Improvements

* Incorporate larger music datasets.
* Support mood-based recommendations.
* Develop a web-based user interface.
* Integrate hybrid recommendation techniques.
* Apply transfer learning using pre-trained audio models.
* Support real-time music recommendation.

---

## Team Information

Team Name: NeuralBeats

Course: Neural Networks Laboratory

Project Title: Music Recommendation System Using Convolutional Neural Networks

---

## License

This project is developed for academic and educational purposes.
