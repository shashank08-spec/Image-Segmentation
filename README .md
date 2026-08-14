# Semantic Image Segmentation using U-Net and DeepLabV3 (ADE20K)

## Project Overview

This project implements semantic image segmentation on a subset of the ADE20K dataset using deep learning techniques. The objective is to classify every pixel in an image into one of five semantic classes:

- Background
- Person
- Car
- Book
- Airplane

The project compares a U-Net model trained from scratch with a DeepLabV3-ResNet50 model initialized with pretrained weights and fine-tuned on the dataset.

---

## Dataset

- Dataset: ADE20K
- Training Images: 350
- Validation Images: 350
- Test Images: 30
- Number of Classes: 5

The dataset was analyzed for:

- Class frequency
- Pixel distribution
- Instance size
- Class co-occurrence
- Data imbalance

---

## Models Implemented

### U-Net

- Trained from scratch
- Encoder-Decoder architecture
- Skip connections
- Cross Entropy Loss with class weights

### DeepLabV3-ResNet50

- Pretrained backbone
- Fine-tuned on ADE20K subset
- Atrous Spatial Pyramid Pooling (ASPP)
- Transfer Learning

---

## Project Workflow

1. Data Loading
2. Exploratory Data Analysis
3. Image Preprocessing
4. Mask Generation
5. Data Augmentation
6. Model Training
7. Model Evaluation
8. Performance Comparison
9. Prediction Visualization

---

## Evaluation Metrics

- Intersection over Union (IoU)
- Dice Score
- Pixel Accuracy
- Mean IoU

---

## Results

The DeepLabV3 model outperformed the U-Net model across all evaluation metrics.

| Model | Description |
|--------|-------------|
| U-Net | Trained from scratch |
| DeepLabV3-ResNet50 | Pretrained and Fine-tuned |

DeepLabV3 achieved significantly better segmentation performance due to transfer learning and a stronger feature extraction backbone.

---

## Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Matplotlib
- Scikit-Learn
- Pillow
- PyCOCOTools

---

## Repository Structure

```
Image-Segmentation/
│
├── notebook/
│   └── ADE20K_Segmentation.ipynb
│
├── report/
│   └── Image_Segmentation_Report.pdf
│
├── images/
│
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

---

## Future Improvements

- Larger training dataset
- Additional semantic classes
- Data augmentation techniques
- Hyperparameter optimization
- Model ensemble methods
- Real-time segmentation

---

## Author

**Shashank Shivakoti**

MSc Data Science

University of Hertfordshire

---

## License

This project is licensed under the MIT License.
