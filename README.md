# ecg-image-classification
design of a proposed hybrid deep learning model of efficientnet and vision transformer


# ECG Classification Using EfficientNet and Hybrid EfficientNet-ViT

This project presents a deep learning pipeline for classifying ECG images into four diagnostic categories using EfficientNet and a hybrid model combining EfficientNet and Vision Transformer (ViT). The pipeline uses PyTorch and HuggingFace Transformers.

---

##  Models Compared

- **EfficientNet-B0** (CNN-based)
- **Hybrid EfficientNet + Vision Transformer (ViT)**

---

## Dataset

The dataset should be structured as follows:

```
ECG_DATA/
├── train/
│   ├── Normal Person ECG Images/
│   ├── ECG Images of Myocardial Infarction Patients/
│   ├── ECG Images of Patient that have abnormal heartbeat/
│   └── ECG Images of Patient that have History of MI/
└── test/
    ├── (same 4 folders as above)
```

**Dataset Source**:  
[Kaggle - ECG Analysis by evilspirit05](https://www.kaggle.com/datasets/evilspirit05/ecg-analysis)

---

## Setup Instructions

### 1. Clone or Download the Repository
```bash
git clone https://github.com/your-username/ecg-classification
cd ecg-classification
```

### 2. Create a Virtual Environment (Recommended)
```bash
conda create -n ecg_env python=3.9
conda activate ecg_env
```

### 3. Install Required Dependencies
```bash
pip install torch torchvision transformers scikit-learn matplotlib seaborn
```

---

## Running the Code

### 1. Launch Jupyter Notebook
```bash
jupyter notebook
```

### 2. Open the file:
```
final code(efficient and hybrid model).ipynb
```

### 3. Modify Dataset Paths
In the notebook, update:
```python
data_dir = "C:/Path/To/ECG_DATA/train"
test_dir = "C:/Path/To/ECG_DATA/test"
```

### 4. Run the Notebook Cell
- Use **Shift + Enter** to execute each cell.
- Models will train for 20 epochs using SGD.
- Training logs, evaluation metrics, and plots will appear inline.

---

## Output

- **Classification Reports** with F1, Recall, Precision
- **Confusion Matrices** for each model
- **Training Loss & Validation Accuracy Curves**
- **Logistic Regression Scatter Plot** of class separability

---

## Notes
- Optimizer used: **Stochastic Gradient Descent (SGD)**. The notebook also includes comparison with Adam.

---

##  Citation

If using this pipeline, please cite the dataset:
```
evilspirit05, 2022. ECG Analysis. Kaggle. Available at: https://www.kaggle.com/datasets/evilspirit05/ecg-analysis [Accessed 27 Apr. 2025].
```

---

## Author

This project was developed by Ikechukwu Ukadike as part of a design of an optimized deep learning model and applied for the purpose of a dissertation on ECG image classification.

