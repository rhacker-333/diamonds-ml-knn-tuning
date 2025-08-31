# Diamonds ML KNN Tuning

## 📌 Project Overview
This repository contains a machine learning project focused on predicting the **cut quality** of diamonds using the **K-Nearest Neighbors (KNN)** classification algorithm.  
The project uses the popular **Diamonds** dataset from the `ggplot2` package in R and demonstrates an end-to-end workflow including:

- Data preprocessing
- Normalization
- Model training
- Hyperparameter tuning
- Final evaluation

---

## 📊 Dataset
The **Diamonds** dataset consists of **53,940 observations** with variables describing physical and quality attributes of diamonds:

- **carat** – Weight of the diamond  
- **cut** – Quality of the cut *(Fair, Good, Very Good, Premium, Ideal)* — **target variable**  
- **color** – Diamond color, from D (best) to J (worst)  
- **clarity** – A measure of how clear the diamond is *(I1 to IF)*  
- **depth**, **table** – Proportional measurements  
- **price** – Price in US dollars  
- **x, y, z** – Physical dimensions in mm  

---

## ⚙️ Methodology
1. Removed categorical predictors (`color`, `clarity`) to simplify initial KNN application.
2. Normalized numeric features to scale all predictors within the same range for unbiased distance calculation.
3. Split the dataset into training and testing subsets.
4. Trained a baseline KNN model.
5. Applied systematic **hyperparameter tuning** for the number of neighbors (`k`) to find the highest test accuracy.
6. Evaluated model performance using a **confusion matrix** and accuracy score.

---

## 🏆 Key Results
- **Best k**: 22  
- **Final Test Accuracy**: ~70.16%  

Given the multi-class nature of the problem and the subtle patterns in the dataset, this accuracy is reasonable for KNN with only numeric predictors.

<img width="533" height="524" alt="image" src="https://github.com/user-attachments/assets/97b29319-0d05-4fb1-ac84-83f0402f6cc7" />

<img width="559" height="542" alt="image" src="https://github.com/user-attachments/assets/69a21750-113e-4ab1-9fab-5a1d2620480c" />

<img width="612" height="540" alt="image" src="https://github.com/user-attachments/assets/346f9f5d-00ad-4b6c-b531-754e0772826d" />


---

## 🚀 Usage
To reproduce the analysis:
1. Clone this repository.
2. Use the `.ipynb` file or  Open the R notebook file after changing its extension  to `.ipynb`
3. Now open the file using Kaggle
4. Run all cells sequentially to reproduce preprocessing, training, tuning, and evaluation steps.

---

## 🔮 Next Steps
Potential enhancements:
- Encode categorical variables (`color`, `clarity`) to include them in the model.
- Feature engineering (e.g., combining `x`, `y`, and `z` into diamond volume).
- Compare with advanced models like **Random Forest** or **Gradient Boosting**.
- Use **cross-validation** for more robust accuracy estimation.

---

## 📄 License
This project is open for educational and personal use.  
Please provide appropriate credit if you use it in your own work.
