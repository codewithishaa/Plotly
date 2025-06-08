### 📘 What I Did in This Notebook

In this notebook, I explored interactive data visualization using **Plotly**, **Cufflinks**, and **Folium** with the following key steps:

---

#### 📦 1. Library Setup
- Installed and imported the following libraries:
  - `plotly`, `cufflinks`, `folium`, `matplotlib`, `seaborn`, `pandas`, `numpy`
- Activated offline mode using `cf.go_offline()` for rendering Plotly plots without internet.

---

#### 📊 2. Data Generation & Preparation
- Used `cf.datagen` utilities to simulate data:
  - `.lines()` → line chart data
  - `.sinwave()` → sine wave for surface plotting
  - `.scatter3d()` and `.bubble3d()` → 3D data simulation
  - `.heatmap()` → matrix-style heatmap data
- Also created custom `DataFrame`s manually and loaded Titanic data using Seaborn.

---

#### 📈 3. 2D Plotting with Cufflinks
- Visualized datasets using:
  - `line`, `bar`, `barh`, `stacked bar`, `area`, `box`, and `histogram` charts via `.iplot()`
- Explored visual styles using:
  - `cf.getThemes()`
  - `cf.set_config_file(theme='polar')` and others

---

#### 🧊 4. 3D Plotting
- Created 3D visualizations using:
  - `kind='surface'` (e.g., from `.sinwave()`)
  - `kind='scatter3d'` and `kind='bubble3d'` (e.g., stock-simulated paths)

---

#### 🔥 5. Heatmaps
- Used `cf.datagen.heatmap(20, 20)` to create a color-coded grid
- Rendered interactive heatmaps with custom color scales like `'spectral'`

---

#### 🌍 6. Map Visualizations
- Created interactive maps using **Folium**:
  - Plotted circular markers with `folium.Circle`
  - Saved maps as HTML files (`mymap.html`)
- Created advanced maps with **Plotly**:
  - `plotly.express.scatter_mapbox` → Top 1000 US cities
  - `plotly.graph_objects.Choroplethmapbox` → US unemployment choropleth

---

#### 🚢 7. Titanic Dataset Analysis
- Loaded the Titanic dataset using `sns.load_dataset('titanic')`
- Aggregated survival counts by gender and visualized them with bar plots

---

#### 🛠️ 8. Utility Commands
- Verified environments with `sys.executable`
- Checked and printed versions of `matplotlib`, `folium`, `seaborn`, etc.
- Used `pip install` commands for on-the-fly installation when needed

---
