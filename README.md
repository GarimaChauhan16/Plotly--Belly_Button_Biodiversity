# Belly Button Biodiversity


## Data Visualization Dashboard


The Belly Button Analysis dashboard is available at https://belly-button-biodiversity-g.herokuapp.com/

![Bacteria by filterforge.com](Images/bacteria_by_filterforgedotcom.jpg)

## Background

The objective of this project is to perform a Full-Stack Data Analysis to build an interactive dashboard exploring the Belly Button Biodiversity Dataset using Plotly.js, Flask and Heroku

## Objectives

### Step 1 - Plotly.js

Use Plotly.js to build interactive charts for your dashboard.

* Create a PIE chart that uses data from your samples route (`/samples/<sample>`) to display the top 10 samples.

  * Use `sample_values` as the values for the PIE chart.

  * Use `otu_ids` as the labels for the pie chart.

  * Use `otu_labels` as the hovertext for the chart.

  ![PIE Chart](Images/pie_chart.png)

* Create a Bubble Chart that uses data from the samples route (`/samples/<sample>`) to display each sample.

  * Use `otu_ids` for the x values.

  * Use `sample_values` for the y values.

  * Use `sample_values` for the marker size.

  * Use `otu_ids` for the marker colors.

  * Use `otu_labels` for the text values.

  ![Bubble Chart](Images/bubble_chart.png)

* Display the sample metadata from the route `/metadata/<sample>`

  * Display each key/value pair from the metadata JSON object somewhere on the page.

* Update all of the plots any time that a new sample is selected.

![Example Dashboard Page](Images/dashboard_part1.png)
![Example Dashboard Page](Images/dashboard_part2.png)


* Adapt the Gauge Chart from <https://plot.ly/javascript/gauge-charts/> to plot the Weekly Washing Frequency obtained from the `/metadata/<sample>`route.

* Modify the example gauge code to account for values ranging from 0 - 9.

* Update the chart whenever a new sample is selected.

![Weekly Washing Frequency Gauge](Images/gauge.png)




## Step 2 - Heroku

Deploy the Flask app to Heroku.


- - -

## Flask API

Use Flask API starter code to serve the data needed for the plots.