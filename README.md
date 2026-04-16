#  World Happiness Report — Data Analysis & Visualization

> A data analysis project by **Nikhil Sahu** exploring what makes nations happy —
> and how factors like GDP, freedom, health, and social support shape well-being across the world.

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![Plotly](https://img.shields.io/badge/Plotly-Interactive%20Charts-3F4F75?logo=plotly)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-F7931E?logo=scikit-learn&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)

---

##  About This Project

This is one of my first end-to-end data science projects, built while learning data analysis and visualization with Python.

I used the **2019 World Happiness Report** dataset (via Kaggle) to explore:
- Which countries are the happiest — and what do they have in common?
- How strongly does wealth (GDP) predict happiness?
- Can machine learning cluster countries by their happiness profile?
- Which factors matter most — and which matter least?

This project helped me practice real-world EDA, correlation analysis, interactive visualization with Plotly, and unsupervised ML with K-Means clustering.

---

##  Key Findings

After running the full analysis, here's what I discovered:

-  **Finland ranked #1** in the world with a happiness score of **7.769**
-  **GDP per capita** had the **strongest correlation** with happiness at **0.79** — wealth matters, but isn't everything
-  **Generosity** was the **weakest factor**, showing almost no correlation with overall happiness scores
-  **K-Means clustering (k=4)** revealed 4 distinct country groups — from high-income, high-happiness nations to low-GDP, low-happiness regions
-  Countries with low freedom scores tended to cluster at the bottom, regardless of their GDP

---

##  Visualizations Generated

| Chart | File | Description |
|---|---|---|
| Correlation Heatmap | `correlation_heatmap.png` | How all features relate to each other |
| Top 20 Countries | `top_countries.png` | Ranked horizontal bar chart |
| GDP vs Happiness | `gdp_vs_happiness.html` | Interactive bubble chart |
| World Map | `world_map.html` | Choropleth map by happiness score |
| Feature Importance | `feature_importance.png` | Factors ranked by correlation |
| Country Clusters | `clusters.html` | K-Means clustering visualization |

---

##  Project Structure

```
world-happiness-analysis/
│
├── data/
│   └── 2019.csv                  # Dataset (download from Kaggle — see Setup)
│
├── outputs/                      # All generated charts & maps
│   ├── correlation_heatmap.png
│   ├── top_countries.png
│   ├── feature_importance.png
│   ├── gdp_vs_happiness.html
│   ├── world_map.html
│   └── clusters.html
│
├── happiness_analysis.py         # Main analysis script
├── requirements.txt              # Python dependencies
├── .gitignore
└── README.md
```

---

##  Setup & Usage

### 1. Clone this repository
```bash
git clone https://github.com/nikhilsahu/world-happiness-analysis.git
cd world-happiness-analysis
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Download the dataset
- Visit [Kaggle — World Happiness Report](https://www.kaggle.com/datasets/unsdsn/world-happiness)
- Download `2019.csv` and place it inside the `data/` folder

### 4. Run the analysis
```bash
python happiness_analysis.py
```

All charts will be saved to the `outputs/` folder. Interactive HTML charts will open in your browser automatically.

---

##  Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.8+ | Core language |
| Pandas & NumPy | Data loading, cleaning, analysis |
| Matplotlib & Seaborn | Static charts & heatmaps |
| Plotly | Interactive charts & world map |
| Scikit-learn | K-Means clustering |


---

##  Author 

**Nikhil Sahu**
Learning data science one project at a time.
- GitHub: https://github.com/nikhilgit27
- Feel free to this repo if you found it useful!

---

##  License

This project is licensed under the [MIT License](LICENSE).

---

##  Acknowledgements

- Dataset: [Kaggle — World Happiness Report](https://www.kaggle.com/datasets/unsdsn/world-happiness)
- Original data: [Gallup World Poll](https://www.gallup.com/analytics/349487/gallup-global-happiness-center.aspx)
