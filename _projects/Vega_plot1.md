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

For the two plots, we use [the dataset here.](https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/building_inventory.csv)

Using HTML tags like below:
```
<vegachart schema-url="{{ site.baseurl }}/assets/json/cars.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/assignment10-hx.json" style="width: 60%"></vegachart>

# Write up

#### A description of what you are visualizing

The left one is to explore the relationship between congress district and county in Illinois. We can know how many congress dictrict areas are located in each county and for each section we could know the number of buildings. And the right one is to show the number of building in each county.

#### What design choices you made?

I used those encoding types quantitative-Q(a continuous real-valued quantity), ordinal-O(a discrete ordered quantity), nominal-N(a discrete unordered category). And I didn't use a color scheme in this plot.

#### Discussion of data transformations

I found there are duplicate rows in this csv file so I used pandas to remove those duplicates. Then I found the remaining has more than 5000 rows, therefore I disabled MaxRowsError for altair.


#### Quotations around any parts of Homework #9

[hw 9 Source](https://starboard.gg/hexiang/he-xiang-assignment9-nm5I9G2)

The histogram is exactly the same plot with previous assignment but all in altair style. I just basiclly convert the javascipt liked code into altair(you can clearly compare the original js code with altair code).


#### Interactivity you chose for this plot

I seperate the number of buildings by its county and congress district in the left plot. By selection certain area, it will interactively show total number of building in each county in the right plot without the consideration of its congress district.


<div class="left">
{% include elements/button.html link="https://github.com/CiliaCuiMsim/ciliacuimsim.github.io/blob/master/assets/json/assignment10-hx.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/CiliaCuiMsim/ciliacuimsim.github.io/blob/master/python_notebooks/hw10_hx.ipynb" text="The Analysis" %}
</div>

