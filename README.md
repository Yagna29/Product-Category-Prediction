# **Product Category Prediction**

## **Overview**  
This project predicts the **product category** based on features like **discounted price, actual price, discount percentage, ratings, and number of reviews** using the **Random Forest Classifier**.  

---

## **Dataset & Features**  
- `discounted_price` – Final price after discount  
- `actual_price` – Original price before discount  
- `discount_percentage` – Discount percentage  
- `rating` – Average customer rating  
- `rating_count` – Number of customer reviews  

### **Feature Engineering**  
✅ **Discount Range:** Categorized `discount_percentage` into groups (0-20%, 20-40%, etc.)  
✅ **Score Metric:** `score = rating × rating_count` to measure product popularity  

---

## **Machine Learning Model**  
**Random Forest Classifier** was used because it:  
✅ Handles large datasets well  
✅ Works with both numerical & categorical data  
✅ Provides high accuracy  

### **Model Performance**  
| Split Ratio | Accuracy | Precision | Recall | F1 Score |  
|------------|---------|----------|--------|----------|  
| **80-20**  | 70.98%  | 71.38%   | 70.98% | 70.85%   |  
| **70-30**  | 67.27%  | 67.55%   | 67.27% | 67.25%   |  
| **75-25**  | 67.84%  | 68.04%   | 67.84% | 67.79%   |  

---

## **How to Run?**  
1. **Clone this repository:**  
   ```bash
   git clone https://github.com/YOUR_GITHUB_USERNAME/Product-Category-Prediction.git
   cd Product-Category-Prediction
