<script src="https://cdn.jsdelivr.net/npm/vega@5"></script>
<script src="https://cdn.jsdelivr.net/npm/vega-lite@5"></script>
<script src="https://cdn.jsdelivr.net/npm/vega-embed@6"></script>

## License Types Visualization


## Visualization 1: Top License Types
This bar chart shows the top 10 most common license types issued. The x-axis represents the license type, and the y-axis shows the number of licenses issued. The x-axis variable of Licenses Type is encoded as a categorical variable, while the y-axis variable of the count of licenses and its color scheme is encoded as a quantitative variable. The graph also uses a sequential blue color scheme that gets darker for larger values. In creating this visualization, the data was transformed by grouping by License Type and taking its count, while also sorting by descending order to improve clarity and show order. 

<div id="chart1" style="width: 100%; height: 500px;"></div>
<script type="text/javascript">
  vegaEmbed('#chart1', 'https://kennyr2711.github.io/chart1.json').catch(console.error);
</script>

---

## Visualization 2: Licenses Issued Over Time
This line chart shows the number of licenses issued over time. The x-axis represents year, and the y-axis shows the number of licenses issued. The x-axis variable of year and y-variable of number of licenses issued was both encoded as quantitative, while the color scheme of license type was encoded as categorical. A tooltip is also encoded with the variables Year, Count, and License Type that provides information when hovering over a point. For color scheme, the visualization uses a categorical color scheme (color assigned by altair) to differentiate between license types. In creating this visualization, the data was transformed by modifying the LastModifiedDate variable to make it parsed as a datetime object to extract Year, and then the data was group by Year and License Type. Lastly, it is sorted in ascending order to ensure a constant change in time in the x-axis.

<div id="chart2" style="width: 100%; height: 500px;"></div>
<script type="text/javascript">
  vegaEmbed('#chart2', 'https://kennyr2711.github.io/chart2.json').catch(console.error);
</script>

---
## Interactivity
For the interactivity in the second visualization, I chose to use a built-in (in the graph) dropdown menu that allows the user to select for a specific license type. This helps the graph become more clear by allowing the user to click on a specific license type they are interested in the graph, and it will filter out to only that specific license type with a more detailed view of the distributon of the count throughout the years. Additionally, users can also hover over specific points in the graph to see the specific date and count of the license at that point.

---


## Links
- [The Data](https://github.com/UIUC-iSchool-DataViz/is445_data/raw/main/licenses_fall2022.csv)
- [The Analysis](https://github.com/kennyr2711/kennyr2711.github.io/blob/main/Workbook.ipynb)
