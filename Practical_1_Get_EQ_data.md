---
title: "Scientific Research Project 7: Exploring earthquake magnitude and frequency using historical seismic records"
author: Dr. Fiona Clubb
date: January 2021
geometry: margin=2cm
output: pdf_document
---
## Part 1: Getting earthquake records

In this project, we're going to use the United States Geological Survey (USGS) Earthquake Hazards Program to explore earthquake catalogues from around the world. We're going to work with a dataset from California in the practicals, but for your assessed project you should choose a different area to analyse.

The USGS Earthquake Hazards program collects information from lots of different seismic networks about earthquake source parameters, such as hypocentres (the location in the earth where a rupture starts), magnitudes, depths, and tectonic summaries. All this information is compiled into a catalog called the _ANSS Comprehensive Earthquake Catalog_ or _ComCat_.

In this first week, we're going to download data for the San Francisco region in California, USA, from _ComCat_. You should follow the steps in this worksheet to download your dataset: **please keep the dataset somewhere safe, as you'll use it in the following weeks**.

### Step 1: Go to the USGS Earthquake Hazards website

Before we start doing any data downloads, first of all explore the USGS website to see what types of data they have available. This is all useful information that you could use for potential dissertation projects. Have an explore of the website:
```
https://www.usgs.gov/natural-hazards/earthquake-hazards/earthquakes
```
### Step 2: Download the historical earthquake data

The main dataset that we are going to use is the _Historical earthquake catalog_. You can access it here:
```
https://earthquake.usgs.gov/earthquakes/search/
```
This website allows you to choose some basic options to filter the earthquakes that you want to download. For this practical, use the following options:

* **Magnitude**: choose a minimum magnitude of 4.5 by clicking the option `4.5+`. This will stop the dataset from being too big by limiting to reasonably large earthquakes.

*  **Date & Time**: this option allows you to set a date range for the earthquakes that you want. We will select all earthquakes that have occurred from 1900 - 2020. In the `Start` box type `1900-01-01 00:00:00`, and in the `End` box type `2020-01-01 00:00:00`. This will select all earthquakes that occurred from midnight on 1st January 1900 to midnight on 1st January 2020.

![](/mnt/c/Users/fclub/OneDrive/Documents/GitHub/SciRes-Earthquakes/figures/practical1_fig1.PNG)

* **Geographic Region**: this allows you to select the area that you want to examine. We will select the area around San Francisco by clicking the orange box that says `Draw Rectangle on Map`. Zoom in to the San Francisco region and click once to choose the start point of your rectangle, then again to finish your rectangle.

![](/mnt/c/Users/fclub/OneDrive/Documents/GitHub/SciRes-Earthquakes/figures/practical1_fig2.PNG)

For now, we don't need to bother with any of the advanced options. The next step is to click on `Output Options` and choose `CSV` to export the data as a `CSV` file. This can be opened in Excel or in Python (our next step.)

![](/mnt/c/Users/fclub/OneDrive/Documents/GitHub/SciRes-Earthquakes/figures/practical1_fig3.PNG)

You can leave the other options as the default. Click `Search`. Your browser should then download a file called `query.csv` which will contain the earthquake data for the San Francisco region.

### Step 3: Rename and save the file somewhere sensible

The final step in downloading the data is to rename the file something more sensible. This is up to you, but it would be best to choose a name that reflects the area and the time frame you have chosen. Right-click on your file and rename it to something like:
```
San_Francisco_earthquakes_1900-2020.csv
```
Now save this file somewhere sensible on your computer, such as on your University storage drive or in the Cloud. **Keep all files from this practical safe: we will be working with these data over the next few weeks**
