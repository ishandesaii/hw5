---
layout: default
title: HW5 Visualization
---

# Homework 5: UFO Sightings Visualized

## 📊 Plot 1: UFO Sightings by Hour of Day

<div id="chart1"></div>

## 🛸 Plot 2: UFO Sightings by Shape

<div id="chart2"></div>

---

### 🔁 Interactivity Discussion

Plot 1 uses brush selection to highlight specific hours of the day. Plot 2 uses an interactive legend to filter sightings by UFO shape. Both interactions allow users to explore the data more clearly and meaningfully.

---

### 🔗 Resources

[📁 The Data](https://github.com/UIUC-iSchool-DataViz/is445_data/raw/main/ufo-scrubbed-geocoded-time-standardized-00.csv)  
[📓 The Notebook](https://github.com/ishandesaii/hw5/blob/main/hw5_notebook.ipynb)

---

## 📈 Visualizations

<script src="https://cdn.jsdelivr.net/npm/vega@5"></script>
<script src="https://cdn.jsdelivr.net/npm/vega-lite@5"></script>
<script src="https://cdn.jsdelivr.net/npm/vega-embed@6"></script>

<script>
vegaEmbed('#chart1', 'assets/chart1.json').catch(console.error);
vegaEmbed('#chart2', 'assets/chart2.json').catch(console.error);
</script>

