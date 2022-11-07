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
For plot 2 built onto the same dataset, we have the visualization as follow:

<vegachart schema-url="{{ site.baseurl }}/assets/json/hw10-cc.json" style="width: 100%"></vegachart>


## Search The Data & Methods


<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/CiliaCuiMsim/ciliacuimsim.github.io/blob/master/assets/json/hw10-cc.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/CiliaCuiMsim/ciliacuimsim.github.io/blob/master/python_notebooks/hw10_cc.ipynb" text="The Analysis" %}
</div>

