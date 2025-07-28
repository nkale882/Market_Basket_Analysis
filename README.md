# 🛒 Market Basket Analysis using Apriori with Hash Tree Optimization

This project applies Market Basket Analysis on a large-scale retail dataset using the **Apriori algorithm**, optimized via **Hash Tree structure** using the `efficient-apriori` library. The goal is to uncover meaningful association rules between products purchased together — ideal for cross-selling, recommendation systems, and inventory decisions.

---

## 📁 Dataset

- Format: `.xlsx` (Excel)
- Records: 5,25,461 rows
- Columns:
  - `Invoice`, `StockCode`, `Description`, `Quantity`
  - `InvoiceDate`, `Price`, `Customer ID`, `Country`

📥 [Download Dataset](https://docs.google.com/spreadsheets/d/1SKIl0OpmkmMtAfZwc7K20CWvvMJGGaGW/edit?usp=sharing&ouid=112213017495102254362&rtpof=true&sd=true)

> Note: The dataset is hosted on Google Drive due to its size. Download and upload it to Colab before running the notebook.


---

## 🎯 Project Goals

- Perform **data preprocessing** on a massive Excel dataset
- Use **Apriori algorithm with Hash Tree** for fast rule mining
- Extract strong **association rules** (support, confidence, lift)
- Provide **product recommendations** based on input
- Visualize patterns with heatmaps, scatter plots, and bar charts

---

## ⚙️ Technologies Used

| Tool        | Purpose                             |
|-------------|-------------------------------------|
| Python      | Core programming                    |
| Pandas      | Data processing                     |
| Seaborn/Matplotlib | Data visualization            |
| `efficient-apriori` | Fast Apriori using Hash Tree |
| Google Colab| Cloud notebook environment          |
| GitHub      | Version control and deployment      |

---

## 📊 Visualizations

- 📈 **Support vs Confidence Scatter Plot**
- 🔥 **Top Rules by Lift (Bar Plot)**
- 🔁 **Item-to-Item Recommendation System**

---

## 🔍 Sample Association Rules

| Rule | Confidence | Support | Lift |
|------|------------|---------|------|
| {POPPY'S PLAYHOUSE KITCHEN} → {POPPY'S PLAYHOUSE BEDROOM} | 70% | 1.2% | 12.5 |
| {72 SWEETHEART FAIRY CAKE CASES} → {PACK OF 60 PINK PAISLEY CAKE CASES} | 42.6% | 1.3% | 10.8 |

---

## 💡 Features

- ✅ Load and preprocess large Excel-based retail data
- 🧠 Rule mining using **Apriori with Hash Tree** (via `efficient-apriori`)
- 📥 User input for generating product recommendations
- 📊 Rich visualizations to explain rule strength
- 🔽 Export results to CSV for use in BI tools
- 🖥️ Interactive recommendation system (CLI-based)

---

## 🧪 Sample Query

```python
Enter a product name: SET/6 RED SPOTTY PAPER PLATES
🛒 Recommended: SET/6 RED SPOTTY PAPER CUPS | Confidence: 78.5% | Lift: 9.2
