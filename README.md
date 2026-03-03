# 🌸 Iris Dataset Clustering using K-Means

---

## 📌 Project Overview

This project applies **unsupervised learning** to the Iris dataset to discover hidden patterns using **K-Means clustering**.

The objectives were to:

- Scale the dataset properly  
- Determine the optimal number of clusters using the Elbow Method  
- Apply K-Means clustering  
- Visualize cluster patterns  

---

## 📊 Dataset Information

The Iris dataset contains:

- **150 samples**
- **4 numerical features:**
  - Sepal Length
  - Sepal Width
  - Petal Length
  - Petal Width
- **3 species** (used only for evaluation, not for training)

Since K-Means is an **unsupervised algorithm**, species labels were not used during clustering.

---

## ⚙️ Steps Performed

### 1️⃣ Data Preprocessing

- Loaded the dataset  
- Checked for missing values  
- Applied feature scaling using **StandardScaler**

Scaling was necessary because K-Means is distance-based and sensitive to feature magnitude differences.

---

### 2️⃣ Finding Optimal K (Elbow Method)

To determine the optimal number of clusters, the **Elbow Method** was used.

**Process:**

- Ran K-Means for K = 1 to 10  
- Calculated Within-Cluster Sum of Squares (WCSS)  
- Plotted WCSS vs K  
- Observed the “elbow” point  

**Result:**  
The optimal number of clusters was found to be **K = 3**.

---

### 3️⃣ Applying K-Means Clustering

K-Means was applied with:

- `n_clusters = 3`  
- Random initialization  
- Multiple runs for stability  

The algorithm grouped the data into 3 clusters based purely on feature similarity.

---

### 4️⃣ Visualization

The clustered data was visualized using scatter plots.

- Each point represents a flower sample  
- Colors represent cluster assignments  
- Visualization was done using 2 selected features / PCA (if applied)

This helped observe natural group separation.

---

## 📈 Observations

- One cluster was clearly separated (corresponding to Setosa)  
- Two clusters had partial overlap (Versicolor and Virginica)  
- Petal measurements contributed strongly to cluster separation  

---

## 🧠 Key Learning Outcomes

- Importance of scaling in distance-based algorithms  
- How to determine optimal K using the Elbow Method  
- Understanding unsupervised pattern discovery  
- Visualizing high-dimensional data  

---

## 🚀 Tools & Libraries Used

- Python  
- NumPy  
- Pandas  
- Matplotlib  
- Seaborn  
- Scikit-learn  

---

## 📌 Conclusion

K-Means clustering successfully identified natural groupings in the Iris dataset.

The experiment demonstrates how unsupervised learning can reveal underlying structure without using labeled outputs.

---

## 👩‍💻 Author

**Vaishnavi Rathi**

---
