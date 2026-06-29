# AI vs Real Image Classification using EfficientNetB0

## Overview

This project presents a deep learning solution for classifying images as **Real** or **AI Generated** using **EfficientNetB0** with Transfer Learning. The model is trained on the AI vs Human Generated Dataset from Kaggle and achieves high classification performance through data augmentation, fine-tuning, and optimization techniques.

The project demonstrates a complete image classification pipeline, including data preprocessing, model training, evaluation, and prediction on custom images.

---

## Features

- Binary Image Classification (Real vs AI Generated)
- Transfer Learning using EfficientNetB0
- Image Data Augmentation
- Batch Normalization and Dropout
- Fine-Tuning of Pre-trained Model
- Early Stopping
- Learning Rate Scheduling
- Model Checkpointing
- Performance Evaluation using Accuracy, Precision, Recall, and AUC
- Prediction on Custom Uploaded Images

---

## Dataset

**Dataset Name:** AI vs Human Generated Dataset

**Source:** https://www.kaggle.com/datasets/alessandrasala79/ai-vs-human-generated-dataset

The dataset contains:

- Real Images
- AI Generated Images
- Training Metadata (train.csv)
- Testing Metadata (test.csv)

---

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Google Colab
- KaggleHub

---

## Model Architecture

- EfficientNetB0 (Pre-trained on ImageNet)
- Data Augmentation
- EfficientNet Preprocessing
- Global Average Pooling Layer
- Batch Normalization
- Dense Layer (256 Units, ReLU)
- Dropout (0.4)
- Dropout (0.3)
- Sigmoid Output Layer

---

## Training Techniques

- Transfer Learning
- Fine-Tuning
- Binary Crossentropy Loss
- Adam Optimizer
- EarlyStopping Callback
- ReduceLROnPlateau Callback
- ModelCheckpoint Callback

---

## Performance

- Validation Accuracy: **93.35%**
- Validation AUC: **98.22%**

---

## Project Structure

```
AI-vs-Real-Image-Classification/
│
├── AI_vs_Real_Image_Classification.ipynb
├── README.md
├── requirements.txt
├── best_model.keras
└── sample_predictions/
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/AI-vs-Real-Image-Classification.git
```

Install the required packages:

```bash
pip install -r requirements.txt
```

---

## Dataset Setup

Download the dataset using KaggleHub:

```python
from kagglehub import dataset_download

path = dataset_download(
    "alessandrasala79/ai-vs-human-generated-dataset"
)
```

Or download it manually from Kaggle and place it in your working directory.

---

## Running the Project

1. Download the dataset.
2. Open the notebook in Google Colab or Jupyter Notebook.
3. Run all cells sequentially.
4. Train the model.
5. Save the best model.
6. Upload any image to classify it as **Real** or **AI Generated**.

---

## Example Prediction

```
Prediction Probability: 0.9642

Prediction: AI Generated Image
```

or

```
Prediction Probability: 0.0418

Prediction: Real Image
```

---

## Future Enhancements

- Improve generalization for newer AI image generators (ChatGPT, Gemini, FLUX, Midjourney, etc.).
- Fine-tune the model using additional modern AI-generated image datasets.
- Develop a web application using Streamlit or Flask.
- Deploy the model as a REST API.
- Extend the model to identify the specific AI generator.

---

## License

This project is intended for educational and research purposes.
