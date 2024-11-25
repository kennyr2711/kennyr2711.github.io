---
title: License Types Visualization
---

## Visualization 1: Top License Types
This static bar chart shows the top 10 most common license types issued. The x-axis represents the license type, and the y-axis shows the number of licenses issued. A sequential blue color scheme was used to emphasize higher counts.

<div id="chart1" style="width: 100%; height: 500px;"></div>
<script type="text/javascript">
  vegaEmbed('#chart1', 'chart1.json').catch(console.error);
</script>

---

## Visualization 2: Licenses Issued Over Time
This interactive line chart visualizes the number of licenses issued over time. Users can interact with the legend to filter the chart by license type.

<div id="chart2" style="width: 100%; height: 500px;"></div>
<script type="text/javascript">
  vegaEmbed('#chart2', 'chart2.json').catch(console.error);
</script>

---

## Links
- [The Data](https://github.com/UIUC-iSchool-DataViz/is445_data/raw/main/licenses_fall2022.csv)
- [The Analysis](https://github.com/kennyr2711/licenses-visualization/blob/main/licenses_visualizations.ipynb)
