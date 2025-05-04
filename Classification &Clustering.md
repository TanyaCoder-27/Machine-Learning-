
---

## **1) Non-Probabilistic Models**
A **non-probabilistic model** is a type of machine learning model that makes predictions without relying on probability distributions. Instead of predicting the likelihood of an outcome, these models use deterministic rules or distance-based metrics to classify data points or find patterns.

### **Examples of Non-Probabilistic Models**:
- **Support Vector Machines (SVM)**: Uses hyperplanes to separate classes without relying on probabilities.
- **K-Nearest Neighbors (KNN)**: Classifies points based on the closest neighbors rather than probability distributions.
- **Decision Trees**: Uses a set of rules to split data into categories without probabilistic calculations.

---

## **2) K-Nearest Neighbors (KNN) Algorithm**
KNN is a simple yet powerful **classification and regression** algorithm. It works by finding the k nearest neighbors to a given query point and determining its class based on the majority vote (for classification) or averaging values (for regression).

### **Steps in KNN**:
1. Choose a value for **K** (number of neighbors).
2. Compute distances from the query point to all training samples.
3. Select the **K** nearest points.
4. Determine the class label using majority voting (classification) or averaging (regression).

### **Example Problem**:
Suppose we have the following dataset:

| Age | Income | Likes Ice Cream (Yes/No) |
|----|--------|-------------------------|
| 25 | 35,000 | Yes |
| 40 | 60,000 | No |
| 30 | 50,000 | Yes |
| 35 | 45,000 | No |

If a new person is **32 years old** and has an **income of 48,000**, we can use KNN to classify whether they "Like Ice Cream" or not by analyzing their nearest neighbors.

---

## **3) Logistic & Linear Regression and Their Differences**
### **Linear Regression**:
- Used for predicting **continuous** values.
- Finds a relationship between independent (X) and dependent (Y) variables using a straight line:  
  $$ Y = mX + c $$

### **Logistic Regression**:
- Used for **classification problems** (binary outcomes).
- Uses the **sigmoid function** to squeeze predictions between 0 and 1:
  $$ f(x) = \frac{1}{1 + e^{-x}} $$

### **Differences**:
| Feature | Linear Regression | Logistic Regression |
|---------|------------------|---------------------|
| Output Type | Continuous (Real Numbers) | Discrete (0/1) |
| Function Used | Linear Equation | Sigmoid Function |
| Use Case | Predict prices, stock values | Spam detection, fraud classification |

---

## **4) K-Means Clustering**
### **Approach**:
K-Means clustering partitions data into **K clusters**, where each data point belongs to the cluster with the nearest centroid.

### **Steps**:
1. Choose the number of clusters **K**.
2. Initialize **K** centroids randomly.
3. Assign each data point to the nearest centroid.
4. Update centroids by calculating the mean of assigned points.
5. Repeat until centroids do not change.

### **Example**:
Consider customer segmentation for a retail store. Given purchase history, K-Means groups customers into clusters like:
- **Budget Shoppers**
- **Premium Shoppers**
- **Frequent Buyers**

### **Advantages**:
✔️ Simple and scalable  
✔️ Works well with large datasets  
✔️ Efficient for clustering applications  

### **Disadvantages**:
❌ Sensitive to initial cluster assignments  
❌ Struggles with varying cluster sizes and densities  
❌ Doesn’t perform well with non-spherical data clusters  

---

## **5) Naïve Bayes Algorithm**
Naïve Bayes is a **probabilistic classifier** based on Bayes’ theorem:

$$ P(A | B) = \frac{P(B | A) P(A)}{P(B)} $$

### **Assumptions**:
- Features are **conditionally independent**.
- Uses prior probabilities to classify new data.

### **Example**:
Spam email detection:
- Words like "WIN", "FREE", "LOTTERY" → High probability of spam.
- Words like "Hello", "Meeting", "Agenda" → Likely not spam.

By calculating probabilities, Naïve Bayes categorizes emails into SPAM or NOT SPAM.

---

## **6) Support Vector Machines (SVM)**
SVM is a **non-probabilistic classification algorithm** that finds a **hyperplane** that best separates different classes.

### **Key Features**:
- **Maximizes margin** between classes.
- Works well with **high-dimensional data**.
- Can handle **non-linearly separable** cases using **kernels**.

### **Example**:
SVM is used in **face detection**, where it classifies faces vs. non-faces by finding the best decision boundary.

---

## **7) Probabilistic Classifiers / Probabilistic Classification Algorithms**
Probabilistic classifiers predict the probability of a sample belonging to a certain class.

### **Common Algorithms**:
1. **Naïve Bayes**: Uses conditional probability (fast and efficient).
2. **Logistic Regression**: Uses sigmoid function for probabilities.
3. **Gaussian Mixture Models (GMM)**: Uses probability distributions to model complex data.
4. **Hidden Markov Models (HMM)**: Used for sequential data like speech recognition.

### **Use Case**:
Probabilistic classifiers are widely used in medical diagnosis where doctors need **confidence scores** for disease prediction rather than a strict binary classification.

---
 😊
