---
name: Vega Lite Example Plot one
tools: [Python, HTML, vega-lite]
image: assets/pngs/plot1.PNG
description: This is the first plot using vega lite for interactive visualization.
author: Xiang He
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Vega chart #1:

```
<vegachart schema-url="{{ site.baseurl }}/assets/json/cars.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/assignment10-hx.json" style="width: 60%"></vegachart>


## Search The Data & Methods
<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com//assets/json/assignment10-hx.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/hw10_hx.ipynb" text="The Analysis" %}
</div>

