# 🔍 Deepfake Image Detection Using Deep Learning

A deep learning-based computer vision project that classifies face images as **Real** or **Fake** using MobileNetV2 transfer learning and TensorFlow/Keras.

## 📌 Project Overview

Deepfake technology can generate or manipulate facial images that appear realistic. This project explores deep learning techniques for distinguishing real and fake face images through binary image classification.

A MobileNetV2-based model is trained and evaluated on a real-versus-fake face image dataset. The project demonstrates image preprocessing, transfer learning, model training, and performance evaluation.

## 🎯 Objectives

* Build a deep learning model for real-versus-fake face image classification.
* Apply image preprocessing for model training.
* Use MobileNetV2 transfer learning for computer vision.
* Evaluate classification performance using standard metrics.
* Document the workflow in a reproducible Jupyter Notebook.

## 🛠️ Technologies Used

* **Programming Language:** Python
* **Deep Learning:** TensorFlow, Keras
* **Model Architecture:** MobileNetV2
* **Data Processing:** NumPy, Pandas
* **Visualization:** Matplotlib, Seaborn
* **Evaluation:** Scikit-learn
* **Development Environment:** Google Colab, Jupyter Notebook

## 📂 Repository Structure

```text
DeepFake-Image-Detection/
│
├── Deepfake_Image_Detection.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## 📊 Dataset

The project uses a real-versus-fake face image dataset.

The dataset contains real and fake face images for binary classification. Dataset files are not included in this repository; refer to the notebook for dataset loading and setup instructions.

Dataset source: [140k Real and Fake Faces — Kaggle](https://www.kaggle.com/datasets/xhlulu/140k-real-and-fake-faces)

## ⚙️ Project Workflow

1. Load and explore the dataset.
2. Prepare image data for model input.
3. Apply preprocessing and label encoding.
4. Implement MobileNetV2-based transfer learning.
5. Train the binary classification model.
6. Evaluate performance on the test dataset.
7. Analyze class-wise precision, recall, and F1-score.

## 🧠 Model Evaluation

The trained model was evaluated on **20,000 test images**.

| Evaluation Metric | Result |
| ----------------- | -----: |
| Test Accuracy     | 77.56% |
| Test Loss         | 0.4795 |
| Macro F1-score    | 77.52% |

### Class-wise Classification Report

| Metric    |   Fake |   Real |
| --------- | -----: | -----: |
| Precision | 75.41% | 80.11% |
| Recall    | 81.79% | 73.33% |
| F1-score  | 78.47% | 76.57% |
| Support   | 10,000 | 10,000 |

### Results Interpretation

The model achieved 77.56% test accuracy on the evaluated dataset. Its recall for fake images was 81.79%, while recall for real images was 73.33%.

These results indicate that the model performs differently across the two classes. Further experimentation may help improve generalization and balance class-wise performance.

*Note: Reported values reflect the saved evaluation outputs in the project notebook.*

## 🚀 How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/MuhammadAbdullahIkram/DeepFake-Image-Detection.git
cd DeepFake-Image-Detection
```

### 2. Install Dependencies

It is recommended to use a compatible Python environment.

```bash
pip install -r requirements.txt
```

### 3. Open the Notebook

Open `Deepfake_Image_Detection.ipynb` in Jupyter Notebook or upload it to Google Colab.

### 4. Configure the Dataset

Follow the dataset setup and loading instructions provided inside the notebook.

### 5. Run the Cells

Execute the notebook cells in order to reproduce the workflow and inspect the available outputs.

## 🔮 Future Improvements

* Experiment with data augmentation and hyperparameter tuning.
* Compare MobileNetV2 with other suitable image classification architectures.
* Improve class-wise precision and recall.
* Evaluate robustness on additional unseen datasets.
* Develop an interactive web application for image predictions.

## ⚠️ Limitations

* Model predictions may be incorrect.
* Performance on one dataset does not guarantee performance on images from other sources.
* Classification scores are not proof that an image is authentic or manipulated.
* This project is intended for educational and experimental purposes.

## 👨‍💻 Author

**Muhammad Abdullah**

Data Science Graduate | AI & Machine Learning

* GitHub: [MuhammadAbdullahIkram](https://github.com/MuhammadAbdullahIkram)

## 📄 License

A license has not yet been specified. Before reusing or distributing this project, review the dataset's license and add an appropriate project license if needed.
