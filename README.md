# 🚦 Traffic Violations Data Mining Project

## 📌 Project Overview  
This project analyzes a dataset of traffic violations using various **data mining techniques**, including **data preprocessing, exploratory data analysis (EDA), clustering, geospatial visualization, and classification modeling**. The goal is to gain insights into **traffic violations** and predict **violation types** based on different features.

---

## 📂 Dataset  
The dataset used in this project is **Traffic_Violations.csv**, which contains traffic stop records with attributes such as:
- **Location** (Geolocation, Latitude, Longitude)
- **Vehicle Details** (Make, Model, Year)
- **Driver Demographics** (Race, Gender, DL State)
- **Violation Type, Arrest Type, and Incident Details**
- **Date and Time of Stop**

---

## 📊 Visualizations & Insights  

### **1️⃣ Violation Type vs Arrest Type Heatmap**
![Violation Type vs Arrest Type](https://github.com/Abhinav-Sriharsha/Traffic-Violation/blob/main/images/Heatmap.png)  
This heatmap shows the **relationship between violation types and the corresponding arrest types**. The color intensity indicates the frequency of occurrences, with lighter shades representing a higher count. It highlights that **citations and warnings** are the most common outcomes.

---

### **2️⃣ Traffic Violations by Hour of the Day**
![Traffic Violations by Hour](https://github.com/Abhinav-Sriharsha/Traffic-Violation/blob/main/images/Hours.png)  
This histogram illustrates **the distribution of traffic violations over 24 hours**. It shows that violations **peak during early morning and late evening hours**, likely due to commuting and nighttime driving patterns.

---

### **3️⃣ Violations by Race and Gender**
![Violations by Race and Gender](https://github.com/Abhinav-Sriharsha/Traffic-Violation/blob/main/images/Race%20and%20Gender.png)  
This bar chart visualizes **traffic violations grouped by race and gender**. It helps identify any potential disparities in violation occurrences among different demographic groups.

---

### **4️⃣ Geospatial Analysis of Traffic Violations**
#### **Seatbelt Violations and Personal Injury-Related Violations**
![Geospatial Analysis of Seatbelt Violations](https://github.com/Abhinav-Sriharsha/Traffic-Violation/blob/main/images/Belts%20and%20Injury.png)  
This map shows the **geographical distribution of seatbelt violations** and **personal injuries**, indicating areas where non-compliance is more frequent.

#### **Alcohol-Related Violations**
![Geospatial Analysis of Alcohol-Related Violations](https://github.com/Abhinav-Sriharsha/Traffic-Violation/blob/main/images/Alcohol.png)  
This plot maps **alcohol-related violations**, showing specific zones with high occurrences of DUI-related offenses.

---

## 🛠️ Steps and Methodologies  

### **1️⃣ Data Preprocessing**
✔️ **Loaded the dataset** using Pandas and removed duplicate records  
✔️ **Handled missing values** by dropping excessive null columns & imputing relevant data  
✔️ **Extracted Latitude & Longitude** from the **Geolocation** column  
✔️ **Converted categorical variables** into numerical values using **Label Encoding**  
✔️ **Transformed `Date Of Stop`** into meaningful time-based features (**Day, Month, Year**)  
✔️ **Derived a new feature:** `Vehicle Condition` based on the year of the vehicle  

---

### **2️⃣ Exploratory Data Analysis (EDA)**
📊 **Key Visualizations:**
- 📌 **Distribution of Traffic Violations by Day of the Week**
- ⏳ **Traffic Violations by Hour of the Day**
- 🚗 **Vehicle Condition Distribution**
- 🔥 **Heatmap of Violation Type vs. Arrest Type**
- 👨‍👩‍👦 **Distribution of Violations by Race & Gender**
  
📊 **Statistical Analysis:**
- **Chi-Squared Tests** to analyze relationships between vehicle conditions and accident-related factors  
- **Feature Correlations** to determine significant attributes  

---

### **3️⃣ Clustering Analysis**
📍 **Applied K-Means Clustering** on geolocation data (`Latitude`, `Longitude`) to identify **high-density** traffic violation areas  
📍 **Visualized Clusters** using scatter plots to highlight hotspots  

---

### **4️⃣ Geospatial Analysis**
🌍 **Used `GeoPandas` and `Shapely`** to create **geographical visualizations** of traffic violations:  
✔️ **Mapped Traffic Violations** using location-based data  
✔️ **Analyzed factors like Personal Injury, Fatal Accidents, and Alcohol Influence**  
✔️ **Identified accident-prone zones and work-zone related violations**  

---

### **5️⃣ Classification Modeling**
📌 Implemented **Supervised Learning Models** to predict the type of violation:
1️⃣ **Logistic Regression**  
2️⃣ **Decision Tree Classifier**  
3️⃣ **Random Forest Classifier**  

📌 **Model Evaluation Metrics:**
✔️ **Classification Report** (Precision, Recall, F1-score)  
✔️ **Accuracy Score Comparison** across models  

---

## 📊 Results & Key Insights
✔️ **Identified peak times** for traffic violations based on **weekday and hour trends**  
✔️ **Geospatial clustering** revealed **violation hotspots**  
✔️ **Vehicle condition** had a strong correlation with **violation frequency**  
✔️ **Random Forest performed best** among all models for violation prediction  

---

## 🛠️ Technologies Used  
- 🟠 **Python** – Data Processing & Analysis  
- 🟡 **Pandas & NumPy** – Data Manipulation  
- 🔵 **Seaborn & Matplotlib** – Data Visualization  
- 🟢 **Scikit-learn** – Machine Learning Models  
- 🔴 **GeoPandas & Shapely** – Geospatial Data Analysis  


