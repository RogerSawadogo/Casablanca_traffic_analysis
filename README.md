
# 🛰️ TTI Analysis Across Communes

This repository contains a complete analysis pipeline to explore and understand **congestion patterns** in various communes using **Travel Time Index (TTI)** data combined with **communal variables** such as population, road infrastructure, transportation facilities, and land use.

---

## 📌 Project Overview

The aim of this project is to:
- Analyze how congestion (via TTI) varies across hours and days of the week.
- Understand how different urban features (e.g., number of highways, population density) correlate with traffic congestion.
- Visualize congestion trends using time series and heatmaps.
- Derive actionable insights to support urban planning and mobility decisions.

---

## 📂 Structure

```
📁 data/                   # Excel files for each day of the week
📁 notebooks/              # Jupyter notebooks for analysis and visualization
📁 plots/                  # Output plots (e.g., correlation heatmaps)
📄 requirements.txt        # Required packages
📄 README.md               # Project documentation (this file)
```

---

## ⚙️ Data Processing

- Merged data from multiple Excel sheets (one per weekday).
- Filled missing commune names and ZIP codes via forward filling.
- Calculated hourly TTI means per commune.
- Pivoted data for time series analysis (communes × hours).
- Computed mean TTI per commune and correlated it with other urban features.

---

## 📊 Key Visualizations

- **Line plots** of hourly congestion by commune.
- **Heatmaps** of average congestion across time.
- **Correlation bar plots** between TTI and features like:
  - 🚋 Tram stations
  - 🚌 Bus stations
  - 🛣️ Number of roads
  - 🏢 Commercial and residential areas

---

## 🔍 Insights

- **Congestion peaks** observed consistently at **8h** and **18h**.
- Positive correlation between **number of tram and bus stations** and congestion.
- Larger **commercial zones** also tend to have higher TTI values.
- Negative correlation between **green/public areas** and congestion in some cases.

---

## 🛠️ Tech Stack

- **Python 3.10+**
- `pandas`, `numpy` for data processing  
- `matplotlib`, `seaborn` for visualization  
- `openpyxl` for Excel handling  
- Jupyter Notebooks for iterative exploration

---

## 🚀 Getting Started

1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/tti-commune-analysis.git
   cd tti-commune-analysis
   ```

2. Create a virtual environment and install requirements:
   ```bash
   python -m venv venv
   source venv/bin/activate  # or venv\Scripts\activate on Windows
   pip install -r requirements.txt
   ```

3. Open notebooks:
   ```bash
   jupyter notebook
   ```

---

## 📈 Future Work

- Extend analysis to **other cities** or **inter-communal** routes.
- Integrate with **geospatial data** for map-based visualizations.
- Build a **dashboard** to interactively explore congestion metrics.

---

## 🤝 Contributing

Feel free to open issues or pull requests! Feedback and collaboration are welcome.

---

## 📄 License

MIT License
