 # **🎵 Music Genre Classification**

This project was developed as part of the Eleveoo Pathways Internship to classify music tracks into genres using both audio features (MFCCs) and spectrogram images.

We explored two main approaches:

Using MFCC features with classical machine learning and dense neural networks.

Using spectrogram images with convolutional neural networks (CNNs).

## **📂 Dataset**

We worked with the GTZAN dataset, which contains:

1000 audio files across 10 genres (30 seconds each).

Pre-extracted features in CSV files (3s and 30s segments).

Spectrogram images generated from the audio files.

The link to the Dataset used: https://www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification/data

## **🚀 Tasks**
### 1. MFCC Feature Extraction

We extracted Mel-Frequency Cepstral Coefficients (MFCCs) from audio files to represent sound in a way similar to human hearing. These features were then used to train machine learning and neural network models.

### 2. CNN on Spectrogram Images

Spectrograms of audio files were generated and used as input to a Convolutional Neural Network (CNN). This approach captures frequency-time patterns in music and significantly improves classification performance.

### 3. Model Training & Validation

Both approaches were trained on a split dataset with training and validation sets. CNNs achieved higher accuracy compared to MFCC-based models.

### 4. Model Evaluation

We evaluated the models using metrics such as accuracy and confusion matrices. CNNs on spectrograms consistently outperformed MFCC-only models.

### 5. Prediction on New Data

The trained model was tested on new spectrogram images to predict their genre. The predictions were displayed alongside the actual spectrogram for visualization.

### 6. Saving the Model

The trained CNN model was saved in both Keras format (.keras) and legacy HDF5 format (.h5) for compatibility.

## **📊 Results**

MFCC-based models: Achieved moderate accuracy, sensitive to dataset balance and feature scaling.

CNN on spectrograms: Achieved significantly better performance, showing the strength of visual features in music genre classification.

## **🛠 Requirements**

Python 3.8+

TensorFlow / Keras

Librosa

NumPy, Pandas, Matplotlib

Scikit-learn

## **🔮 Future Work**

Explore larger datasets such as FMA (Free Music Archive).

Use transfer learning with pre-trained models (ResNet, VGG) on spectrograms.

Deploy the model as a web application for real-time genre prediction.
