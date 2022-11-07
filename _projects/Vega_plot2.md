---
name: Vega Lite Example Plot two
tools: [Python, HTML, vega-lite]
image: assets/pngs/plot2.png
description: This is the second plot using vega lite for interactive visualization.
author: Cilia Cui
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Vega chart #2:
For the two plots, we use [the dataset here.](https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/building_inventory.csv)


For plot #2 built onto the same dataset, we have the visualization as follow:

<vegachart schema-url="{{ site.baseurl }}/assets/json/hw10-cc.json" style="width: 100%"></vegachart>

# Write up

#### A description of what you are visualizing

This plot is a visualization of the distribution of constructions in different floors built by different agencies. The rectangular plot shows the number of constructions that each agency built in different floor levels. The deeper the color is, the more the number of constructions of this floor level that this agency has built.

#### What design choices you made?

To build this plot, I utilized the maxbin of 20 as for the x axis, and applied ordinal type onto the y axis to build a clear view on the different agency names. As for the color, I don't apply a specific color theme onto this plot because there's not a strong reason to do so based on this relatively small data/type scale.
 
#### Discussion of data transformations

In the notebook, I've already check the na values that might affect the visualizaiton effect and found no need to filter the data before applying it to altair. So there's only value checks without data transformations.


#### Quotations around any parts of Homework #9

Acutally this plot is based on my work at [homework #9.](https://starboard.gg/qc23/homework9_qc23-na1PBCyr)
The rec plot is exactly the same plot as the "2 rectangular plot" but in altair style. I just basiclly convert the javascipt liked code into altair(you can clearly compare the original js code with altair code).


#### Interactivity you chose for this plot

See plot 1. In this plot we don't apply the interactive part to it.

<div class="left">
{% include elements/button.html link="https://github.com/CiliaCuiMsim/ciliacuimsim.github.io/blob/master/assets/json/hw10-cc.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/CiliaCuiMsim/ciliacuimsim.github.io/blob/master/python_notebooks/hw10final.ipynb" text="The Analysis" %}
</div>

