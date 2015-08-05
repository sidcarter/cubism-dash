Original
========

The original repo is [here](https://github.com/jefffm/cubism-dash). I've made some modifications to make it work with the metrics pushed via statsd into graphite, upgraded versions and added some bells and whistles

cubista
=======

A cubism wrapper for displaying Graphite data, using bootstrap.

Plug in your graphite URL, edit the JSON object with your graphite metrics, and off you go--you'll have a pretty autorefreshing set of horizon charts grouped by datacenter and role. 

Currently this requires specific Graphite metric namespacing. It should be easy to modify for other uses.

Sample
------

![Screenshot](https://github.com/sidcarter/cubista/blob/master/screenshots/dashboard.png)


This type of chart is especially useful for identifying anomalies. Here's an example--clearly something weird is going on with this role. Other ways of visualizing this data (ie. a line chart with n lines) will sometimes make it difficult to see things like this. Cubism's horizon charts are a great way of mashing up time series data with something close to a heatmap:

![Details](https://github.com/sidcarter/cubista/blob/master/screenshots/zoomed.png)
