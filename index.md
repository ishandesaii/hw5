---
layout: default
title: HW5 Visualization
---

# 🛸 Homework 5: UFO Sightings Visualized

---

## 📊 Plot 1: UFO Sightings by Hour of Day

Chart 1 shows the distribution of UFO sightings across the 24 hours in a day. This interactive histogram helps uncover temporal patterns — for example, whether more sightings happen at night. I extracted the hour from each `sighting_datetime` using Pandas' `.dt.hour` to enable this analysis.

I used a histogram format with hour on the x-axis and count of sightings on the y-axis. Bars are colored conditionally: those within a selected time range are highlighted in **steel blue**, while the rest appear in **light gray**. Users can brush over the x-axis to focus on specific time windows, making it easy to explore trends like evening vs early morning activity.

<div id="chart1" style="margin-top: 20px;"></div>

---

## 🔷 Plot 2: UFO Sightings by Shape

Chart 2 visualizes the number of UFO sightings categorized by the **reported shape** of the object (e.g., circle, disk, light). It uses a bar chart with `shape` on the x-axis and count on the y-axis to show how frequently different shapes are reported.

This chart includes a **clickable legend**, letting users highlight a specific shape. The selected shape stays in color, while others fade to gray, keeping the view clean and focused. I ensured the shape column was treated as a nominal variable and cleaned missing values. Unlike the time-based view in Chart 1, this plot offers insight into the nature of the sightings.

<div id="chart2" style="margin-top: 20px;"></div>

---

## 🔁 Interactivity Discussion

- 🟦 **Plot 1** uses a brush selection to highlight specific hours of the day.
- 🟩 **Plot 2** includes a clickable legend to filter sightings by UFO shape.

These interactive elements improve clarity, allowing users to explore the data from different perspectives more meaningfully.

---

## 🔗 Resources

- [📁 The Data](https://github.com/UIUC-iSchool-DataViz/is445_data/raw/main/ufo-scrubbed-geocoded-time-standardized-00.csv)  
- [📓 The Notebook](https://github.com/ishandesaii/hw5/blob/main/hw5_notebook.ipynb)


<script src="https://cdn.jsdelivr.net/npm/vega@5"></script>
<script src="https://cdn.jsdelivr.net/npm/vega-lite@5"></script>
<script src="https://cdn.jsdelivr.net/npm/vega-embed@6"></script>

<script>
vegaEmbed('#chart1', 'assets/chart1.json').catch(console.error);
vegaEmbed('#chart2', 'assets/chart2.json').catch(console.error);
</script>


