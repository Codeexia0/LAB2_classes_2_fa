# Speech Intelligibility Prediction with CNN and RCNN

This repository contains code for predicting speech intelligibility using deep learning models based on the Clarity Prediction Challenge ([CPC1](https://claritychallenge.org/docs/cpc1/cpc1_intro)) dataset.

This work was part of a B.Sc. thesis that aimed to investigate and develop neural networks for speech intelligibility prediction, achieving better results than the traditional STOI model.

---

## Overview

The project focuses on utilizing Convolutional Neural Networks (CNN) and Recurrent Convolutional Neural Networks (RCNN) to predict how intelligible speech is to human listeners, especially in noisy environments.

### Why Spectrograms and Cochleograms?

- **Spectrograms**: A spectrogram represents the frequency spectrum of the audio signal as it varies with time. It provides a time-frequency representation that allows the model to capture the spectral features of the speech signal. Since speech intelligibility is influenced by the patterns of these spectral features, spectrograms are a natural choice for input to the model.
  
- **Cochleograms**: Cochleograms are derived from the cochlear filterbank, mimicking how the human ear processes sound. These provide a more biologically-inspired representation of sound, which can be more robust to noise and distortions. Cochleograms preserve both time and frequency information while providing a better feature representation for speech intelligibility prediction, particularly in noisy environments.

By using both spectrograms and cochleograms, we provide the model with different ways of interpreting the speech signal, which improves its ability to predict speech intelligibility under various conditions.

---

## Models

Three deep learning models were implemented and compared for speech intelligibility prediction:

### 1. **CNN v1**: A simple CNN model trained on spectrograms or cochleograms.
  - **Diagram for CNN v1** (Add your diagram here)

### 2. **CNN v2**: A more advanced CNN model that showed improved accuracy compared to CNN v1.
  - **Diagram for CNN v2** (Add your diagram here)

### 3. **ResCNN**: A residual CNN model for improved feature learning and performance.
  - **Diagram for ResCNN** (Add your diagram here)

The best model was selected based on performance metrics (e.g., RMSE, CC) and computational efficiency, with **CNN v2** offering the best balance of accuracy and training time.

---

## Experimentation

The models were trained and evaluated on the CPC1 dataset, and various hyperparameters and architectural configurations were tested to optimize performance.

### Key Results

- **CNN v2 with spectrogram input** achieved the best performance, offering an optimal balance between accuracy and training time.
- **ResCNN** had the longest training time, but it offered promising performance, especially for deeper feature learning.
- **CNN v1** was faster but less accurate compared to CNN v2.

---

## Conclusion

This work demonstrated that CNN and RCNN models could significantly improve speech intelligibility prediction compared to traditional methods like STOI. The experiments showed that CNN v2 with spectrogram input offered the best trade-off between performance and computational efficiency.

Future work could explore hybrid models combining CNNs and RNNs or experiment with other feature extraction techniques.

---

## Acknowledgements

This work was part of the Clarity Prediction Challenge 1 (CPC1) and was based on the dataset provided by [The Clarity Project](https://claritychallenge.org).
