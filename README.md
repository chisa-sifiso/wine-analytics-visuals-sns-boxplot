📄 README.md
# 🍷 Wine Analytics Visuals

This project explores the **Wine Reviews dataset** (`winemag-data-130k-v2.csv`) using **Python**, **Pandas**, **Matplotlib**, and **Seaborn**.  
It focuses on analyzing and visualizing wine **prices** and **ratings** across countries.

---

## 📊 Visualizations

1. **Wine Price Distribution**
   ```python
   dataset["price"].hist(bins=2, color="orange")


Shows the distribution of wine prices in the dataset.

Wine Price Distribution by Country

sns.boxplot(x="country", y="price", data=dataset)


Compares wine price ranges across different countries.

Focused Comparison: Italy, Portugal, and US

top_countries = ["Italy", "Portugal", "US"]
subset = dataset[dataset["country"].isin(top_countries)]
sns.boxplot(x="country", y="price", data=subset)


Highlights the price distributions of the top 3 selected countries.

⚙️ Tools & Libraries

Python 3

Pandas

Matplotlib

Seaborn

📂 Project Structure
wine-analytics-visuals/
│── data/
│   └── winemag-data-130k-v2.csv   # dataset
│── analysis.py                    # main Python script with plots
│── visualizations.ipynb           # optional Jupyter Notebook
│── README.md

🚀 How to Run

Clone the repo:

git clone (https://github.com/chisa-sifiso/wine-analytics-visuals-sns-boxplot/blob/main/README.md)
cd wine-analytics-visuals


Install dependencies:

pip install pandas matplotlib seaborn


Run the script:

python analysis.py

📷 Sample Outputs

Price Distribution


Wine Price by Country


📌 Notes

The dataset (winemag-data-130k-v2.csv) must be inside the data/ folder.

Works in both Jupyter Notebook and Python scripts.
