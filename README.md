# Customer Segmentation using K-Means Clustering

## Project Overview
This project implements a **K-Means Clustering** algorithm to group customers of a retail store based on their purchase history. The goal is to identify distinct customer segments to better understand purchasing behavior and target specific groups with marketing strategies.

## Dataset
The project uses the `Mall_Customers.csv` dataset, which contains the following features:
- **CustomerID**: Unique ID for each customer.
- **Gender**: Gender of the customer.
- **Age**: Age of the customer.
- **Annual Income (k$)**: Annual Income of the customer in thousands of dollars.
- **Spending Score (1-100)**: Score assigned by the retail store based on customer behavior and spending nature.

## Dependencies {
To run this project, you need the following Python libraries:
- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn

You can install them using pip:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

## How to Run
1. Ensure `Mall_Customers.csv` is in the same directory as the notebook.
2. Open `Customer_Segmentation.ipynb` in Jupyter Notebook, JupyterLab, or VS Code.
3. Run all cells to process data, train the model, and visualize clusters.

## Implementation Details
1. **Data Loading & EDA**: Loaded the dataset and visualized distributions of income and spending scores.
2. **Feature Selection**: Selected `Annual Income` and `Spending Score` for 2D clustering.
3. **Elbow Method**: Calculated WCSS for K=1 to 10 to determine the optimal number of clusters. The Elbow plot suggested **K=5**.
4. **Model Training**: Trained the K-Means model with 5 clusters.
5. **Evaluation**: Calculated Silhouette Score to assess cluster quality.
6. **Results**: Visualized the 5 customer segments:
    - Low Income, Low Spending
    - Low Income, High Spending
    - Average Income, Average Spending
    - High Income, Low Spending
    - High Income, High Spending

## Conclusion
The analysis successfully identified distinct customer groups. The "High Income, High Spending" group is the most valuable segment for targeting marketing campaigns.
