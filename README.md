# **Evaluation Task: High Granularity Quantization for CICADA**

## **📌 Overview**
This repository contains my submission for the evaluation task on **High Granularity Quantization for CICADA**. The objective was to analyze the dataset, evaluate the given model, and attempt to develop a better-performing model.

## **🛠️ Approach**
The task required understanding the dataset, identifying whether the problem was classification or regression, and improving the existing model if needed. The following steps were taken:

---

## **1️⃣ Understanding the Dataset**

### **📂 Given Files:**
- `data/images.npy` → Image data.
- `data/labels.npy` → Corresponding labels.
- `model/` → Pre-trained model for evaluation.

### **📌 Steps Taken:**
1. Loaded the dataset and checked its structure.
2. Visualized sample images to understand their format.
3. Examined the distribution of labels to assess class balance.

### **🔍 Key Observations:**
- The images were grayscale with dimensions **16×16 pixels**.
- Labels had values `0` or `1`, suggesting a **binary classification problem**.

---

## **2️⃣ Determining the Type of Problem**
A key step was deciding whether the task was classification or regression.

### **🔍 How It Was Identified as Classification:**
✔ Labels were discrete (`0` or `1`), not continuous values.  
✔ No clear regression objective was present.  
✔ The dataset structure was similar to common classification tasks.

📢 **Conclusion:** The task was identified as **binary classification** based on label characteristics.

---

## **3️⃣ Evaluating the Given Model**

### **📌 Steps Taken:**
1. Loaded the provided model.
2. Checked its architecture and input requirements.
3. Resized images to match the expected input dimensions.
4. Ran predictions and analyzed model performance.

### **⚠ Issues Found:**
- The model was **biased towards class `1`**, predicting `1` in most cases.
- Accuracy was low, suggesting poor classification performance.

📢 **Conclusion:** The existing model had significant limitations, making improvements necessary.

---

## **4️⃣ Improving the Model**

### **Key Considerations:**
✔ Adjusted feature extraction techniques.  
✔ Applied strategies to improve generalization.  
✔ Ensured proper activation functions were used for classification.

---

## **5️⃣ Training & Evaluation**

### **Training Approach:**
- Used an appropriate loss function for classification.
- Applied optimization techniques to enhance learning.
- Considered early stopping to prevent overfitting.

---

## **6️⃣ Performance Analysis**

### **📌 Evaluation Criteria:**
- Standard classification metrics were used.
- Comparison with the initial model was made.
- Overfitting was monitored due to the small dataset size.

📢 **Conclusion:** The modifications aimed to enhance the model’s ability to generalize better.

---

## **7️⃣ Saving and Reproducibility**
To ensure the model could be reused, it was saved for future evaluation and testing.

---

## **📢 Conclusion**
### **✅ Summary of Work Done:**
- Analyzed the dataset and identified the nature of the problem.
- Evaluated the given model and its limitations.
- Developed an improved approach to enhance performance.
- Ensured reproducibility of the process.

