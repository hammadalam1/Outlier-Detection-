# 📊 Outlier Detection Using Z-Score and IQR in Python

This project demonstrates how to detect **outliers** in a dataset using two statistical methods:  
- **Z-Score Method**  
- **IQR (Interquartile Range) Method**

The results are visualized using scatter plots with outliers highlighted in red.

## 🧠 Methods Used

### 🔹 1. Z-Score Method
- Calculates how far each data point is from the mean in terms of standard deviations.
- Data points with a Z-score above a threshold (e.g., `|z| > 2`) are marked as outliers.

### 🔹 2. IQR (Interquartile Range) Method
- Uses the 25th percentile (Q1) and 75th percentile (Q3) to calculate the IQR.
- Any value below `Q1 - 1.5 * IQR` or above `Q3 + 1.5 * IQR` is flagged as an outlier.


## 🧪 Dataset

data = np.array([3, 6, 2, 9, 5, 6, 6, 13, 11, 1, 16, 14, 41, 56])

📦 Requirements
Install the necessary Python libraries:
pip install numpy matplotlib scipy

▶️ How to Run
Copy the code into a Python file (e.g., outlier_detection.py)

Run the script:

 outlier_detection.py
Two plots will appear:

Outliers detected using Z-Score

Outliers detected using IQR

📈 Sample Output
Blue dots = Inliers

Red dots = Outliers

Z-Score Plot:
Identifies points far from the mean based on standard deviation.

IQR Plot:
Highlights points outside the interquartile range.

🧮 Libraries Used
numpy – for numerical calculations

scipy.stats.zscore – for Z-score calculation

matplotlib.pyplot – for plotting data



✍️ Author
Hammad Alam