---
layout: default
title: Lab 6 - Vector Analysis
description: Learn how to analyze vector data in QGIS
permalink: /labs/lab06/start
active: True
nav: False
multi: True
prev: NULL
next: part1
---
# Lab 6 - Vector Analysis
*Estimated time to complete: 1 hour*

## Goals  
* Use intermediate level tools in QGIS
* Perform basic analysis with vector datasets
* Summarize the results of an analysis in a Map Layout
* _Bonus_: Create a creative and unique map layout

## Key Performance Indicators

* **KPI 1**: Add point data from a table
* **KPI 2**: Use the select within distance tool
* **KPI 3**: Create a buffer around a vector layer
* **KPI 4**: Join attributes by location
* **KPI 5**: Apply skills from previous labs

## Requirements  
* QGIS
* Microsoft Word
* Data Files from eLearning:
    - `dallas_county_UTM14N.gpkg`
    - `Dallas_population_centroids_UTM14N.gpkg`
    - `TRI_sites_TX_UTM14N.csv`

## Optional  
* A computer mouse (separate from a laptop track pad) for easy map navigation

* Additional graphic design software like PowerPoint, Google Slides, Canva, Paint, etc.

## Lab Overview

This lab consists of **seven** parts:
- Project Setup  
- Add Point Data From a Table
- Use the Select Within Distance Tool  
- Create a Buffer Layer
- Join Attributes by Location  
- Make a Map Layout
- Submit your lab 

Please complete each part in order and submit your lab report before the due date.

The lab will be graded based on the Key Performance Indicators (KPIs):

|KPI	|Requirements	|Points|
|---|---|---|
|//|	Completion of this Checklist	|2|
|//|	First and Last name written in the header of your lab report	|2|
|//|	Map layout is submitted as a high-resolution PDF file, professionally formatted and generally legible	|6|
|1|	Add point data from a table – Toxic Release Sites visible in correct locations 	|10|
|2 |	Only sites within 1 mile of Dallas County are visible, and total number of sites within 1 mile is written on the layout	|10|
|3|	1 mile buffer around sites	|10|
|4a|	Buffer is color coded by total population within its area	|10|
|4b|	Number of sites within Dallas County written on the layout	|5|
|5a|	Total population living within buffered areas written on the layout	|5|
|5b|	Base map is visible on the map and legend	|10|
|5c|	Dallas county has a transparent fill (Base map is visible inside the county), TR sites have a non-circle shaped symbol, and all layers are named correctly	|10|
|5d|	Scale bar (in miles), north arrow, legend, and CRS included on map	|10|
|5e|	Title, author, date, and data source included on the layout	|10|


## Set Up

Create a folder called `lab06` in your digital-earth folder on your computer and save the [Lab 6 report document](https://utdallas.box.com/v/2307-lab6-report) and [data folder](https://utdallas.box.com/v/2307-lab6-data) to this folder. Make sure the extract (unzip) the `data.zip` folder.

[Example Layout](https://utdallas.box.com/v/2307-lab6-example)

Before starting the lab:

* Familiarize yourself with the Toxic Release Inventory data published by the EPA
	* [https://www.epa.gov/toxics-release-inventory-tri-program](https://www.epa.gov/toxics-release-inventory-tri-program)

* Review Scientific Notation and E notation  
	* [https://en.wikipedia.org/wiki/Scientific_notation](https://en.wikipedia.org/wiki/Scientific_notation)
	
