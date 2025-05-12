# 🛍️ FoodMart Data Analysis and Logistic Regression Project

This project analyzes the FoodMart dataset, performs preprocessing, visualization, and builds predictive models using **Simple** and **Multiple Logistic Regression** to understand **home delivery service** behavior. It also applies **K-Medoids** and **Hierarchical Clustering** to explore store patterns.

---

## 📂 Dataset

- **Source:** `StoresData.xlsx`
- Contains store-level information including:
  - Sales, wages, advertising budget
  - Manager demographics and training
  - Store location, unionization, delivery status, competitors, etc.

---

## 📊 Data Preprocessing

### ✔️ Load and Clean Data
```python
df = pd.read_excel('StoresData.xlsx')
df = df.drop(columns=["Sundays", "Mng-Sex", "HomeDel", "Location", "State"])
