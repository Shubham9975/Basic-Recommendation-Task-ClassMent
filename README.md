# 🚀 Basic Recommendation Engine

## 📌 Overview
This project is a simple **Job Role Recommender** that suggests the **top three most similar job roles** based on skills. It uses **Jaccard Similarity** to compare skill sets and find the closest matching roles.

## 📊 Approach/Methodology
📌 The dataset consists of **job roles and their associated skills**.  
📌 Converted data into a **dictionary** for **faster lookup** and stored skills as **sets** for easy comparison.  
📌 Used **MultiLabelBinarizer** to transform skills into **binary vectors** for similarity calculations.  
📌 Used **Jaccard Similarity** for computing similarity:  

J(A, B) = |A ∩ B| / |A ∪ B|

📌 **Intersection (∩)**: Common elements between A and B.  
📌 **Union (∪)**: Unique elements between A and B.  

📌 The top **three most similar job roles** are recommended based on Jaccard Similarity scores.

## 🎯 Why Jaccard Similarity?
✅ **Best for categorical data** – handles **unique, separate values** like skills.  
✅ **Better than Cosine Similarity**, which focuses on frequency rather than presence/absence.  
✅ **Higher Jaccard Similarity → More overlapping skills** → **Better recommendations**.  

This approach ensures a **simple yet effective recommendation engine** for job roles based on required skills.  

## 📝 Explanation
📌 **Dataset Processing**: Stored in a **dictionary** for fast lookup, with **sets for easy comparison**.  
📌 **Binary Representation**: Used **MultiLabelBinarizer** to convert skills into **binary vectors**.  
📌 **Similarity Calculation**: Used **Jaccard Similarity** to measure similarity between skill sets.  
📌 **Final Ranking**: Sorted roles by **similarity scores** and recommended the **top three roles**.

## ⚙️ How to Run
1️⃣ **Clone this repository**  
   ```sh
   git clone https://github.com/Shubham9975/Basic-Recommendation-Task-ClassMent.git
   cd Basic-Recommendation-Task-ClassMent
