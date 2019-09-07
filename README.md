https://biodiversity-kp.herokuapp.com/
## Deployed html with HEROKU
![page1](https://user-images.githubusercontent.com/46768393/64025369-86038580-cb0a-11e9-932d-41c49de5c460.png)


## Sample graph
![sample 163 graph](https://user-images.githubusercontent.com/46768393/64025374-8b60d000-cb0a-11e9-83d0-aeb9b7dd7a2f.png)


## Step 1 - Plotly.js

Use Plotly.js to build interactive charts for your dashboard.

* Create a PIE chart that uses data from your samples route (`/samples/<sample>`) to display the top 10 samples.

  * Use `sample_values` as the values for the PIE chart.

  * Use `otu_ids` as the labels for the pie chart.

  * Use `otu_labels` as the hovertext for the chart.

 ![pie_chart](https://user-images.githubusercontent.com/46768393/62843448-d9ab4d80-bc87-11e9-9dcc-7755d4fe9c37.png)

* Create a Bubble Chart that uses data from your samples route (`/samples/<sample>`) to display each sample.

  * Use `otu_ids` for the x values.

  * Use `sample_values` for the y values.

  * Use `sample_values` for the marker size.

  * Use `otu_ids` for the marker colors.

  * Use `otu_labels` for the text values.

  <img width="1416" alt="bubble_chart" src="https://user-images.githubusercontent.com/46768393/62843518-550cff00-bc88-11e9-8653-83042eb6afe0.png">

* Display the sample metadata from the route `/metadata/<sample>`

  * Display each key/value pair from the metadata JSON object somewhere on the page.

* Update all of the plots any time that a new sample is selected.

* You are welcome to create any layout that you would like for your dashboard. An example dashboard page might look something like the following.

![dashboard_part1](https://user-images.githubusercontent.com/46768393/62843614-1f1c4a80-bc89-11e9-9494-1ed3b30e791b.png)


![dashboard_part2](https://user-images.githubusercontent.com/46768393/62843615-23486800-bc89-11e9-8df1-14465795e6d3.png)

## Step 2 - Heroku

Deploy your Flask app to Heroku.

* You can use the provided sqlite file for the database.

* Ask your Instructor and TAs for help!

- - -

# Advanced Challenge Assignment (Optional)

The following task is completely optional and is very advanced.

* Adapt the Gauge Chart from <https://plot.ly/javascript/gauge-charts/> to plot the Weekly Washing Frequency obtained from the `/metadata/<sample>`route.

* You will need to modify the example gauge code to account for values ranging from 0 - 9.

* Update the chart whenever a new sample is selected.

<img width="384" alt="gauge" src="https://user-images.githubusercontent.com/46768393/62843554-a3ba9900-bc88-11e9-8ddb-4104c0eb1fe4.png">

- - -

## Flask API

Use Flask API starter code to serve the data needed for your plots.

* Test your routes by visiting each one in the browser.

- - -

## Hints

* Don't forget to `pip install -r requirements.txt` before you start your server.

* Use `console.log` inside of your JavaScript code to see what your data looks like at each step.

* Refer to the [Plotly.js Documentation](https://plot.ly/javascript/) when building the plots.

- - -

### Copyright

Data Boot Camp © 2018. All Rights Reserved.
