# MINI PROJECT FUNDAMENTAL ML - Nhóm 4CE

> [!IMPORTANT]
> In this project, we aim to classify images by first using **Principal Component Analysis (PCA)** for dimensionality reduction. PCA helps in transforming the images into a lower-dimensional space while preserving as much variance as possible. After the dimensionality reduction, we will classify the images using a Machine Learning Model, specifically a **Multi-Layer Perceptron (MLP)**. Additionally, we plan to explore **Convolutional Neural Networks (CNN), Histogram of Oriented Gradients (HOG)** as further work.

> [!NOTE]
> You can go to the url https://thangbuiq.github.io/NMMH-4CE for easily view of this file.

## Team Members

| Name               | Student ID | Responsibilities                                                                                   |
|--------------------|------------|----------------------------------------------------------------------------------------------------|
| Bùi Quang Thắng   | 21280048   | Leader, ensure timely completion, integrating all parts of the project and compiling the final report |
| Lê Võ Bảo Trâm     | 21280052   | Handle EDA for each label, and apply XgBoost, MLP, and Naive Bayes classification                     |
| Huỳnh Thị Thu Thoảng | 21280074  | Apply Random Forest, MLP classification, compare time and visualize before and after PCA  |
| Nguyễn Thuý Vy     | 21280120   | Apply Desicion Tree, SVM algorithms with PCA, non PCA and GridSearchCV. Compare score as bar chart    |

## Methodology tl;dr

- Feature Engineering: PCA to reduce the dimensionality while preserving variance (95% cut-off)
- Core ML Algos: Multi-Layer Perceptron (MLP), Random Forest, XgBoost, Naive,... and PCA comparison
- Further work: Convolutional Neural Networks (CNN) for improved classification accuracy

## Model Evaluation and Results

### Original Data
- **Decision Tree**
  - Accuracy: 0.3096
  - Precision: 0.2848
  - Recall: 0.3096
  - F1-Score: 0.2835
- **Random Forest**
  - Accuracy: 0.4631
  - Precision: 0.5184
  - Recall: 0.4631
  - F1-Score: 0.4327
- **SVM**
  - Accuracy: 0.5671
  - Precision: 0.5716
  - Recall: 0.5671
  - F1-Score: 0.5665
- **MLP**
  - Accuracy: 0.4524
  - Precision: 0.4459
  - Recall: 0.4524
  - F1-Score: 0.4420

### PCA-Transformed Data
- **Decision Tree**
  - Accuracy: 0.3098
  - Precision: 0.2888
  - Recall: 0.3098
  - F1-Score: 0.2701
- **Random Forest**
  - Accuracy: 0.4078
  - Precision: 0.5361
  - Recall: 0.4078
  - F1-Score: 0.3601
- **SVM**
  - Accuracy: 0.3142
  - Precision: 0.7015
  - Recall: 0.3142
  - F1-Score: 0.2261
- **MLP**
  - Accuracy: 0.4734
  - Precision: 0.4612
  - Recall: 0.4734
  - F1-Score: 0.4615

### Conclusion
SVM achieved the best performance among the evaluated models. PCA helped reduce computational time significantly but generally resulted in lower performance metrics. Future work will explore CNNs for potentially better accuracy.

### Further Work
- **XGBoost**: Achieved 50% accuracy.
- **CNN**: Achieved 56% accuracy.
