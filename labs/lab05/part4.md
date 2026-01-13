---
layout: default
title: Digital Elevation Models (DEM)
description: ...
permalink: /labs/lab05/part4
active: True
nav: False
multi: True
prev: part3
next: part5
---

# How to Download a Digital Elevation Model (DEM)
Make sure you have installed the OpenTopography DEM Downloader plugin before starting.

<span class='alert'>Make sure you have set a **Projected CRS** before starting!</span>


1. Click **Raster &gt; OpenTopography DEM &gt; OpenTopography DEM Downloader**

    ![](part4_images/screenshot.webp)


2. In the **DEM Downloader** window, select **SRTM 30m** DEM to download.

    Define the extent to download by clicking the small arrow on the right then selecting **Calculate from Layer &gt; satellite_image**

    Enter your API key you got from [opentopography.org](http://opentopography.org) 

    Use the three dots "..." to select the location for the Output raster

    Make sure the **Open output file after running algorithm** option is checked.

    Click **Run**

    ![](part4_images/user_cropped_screenshot.png)


3. Click **Close** once the download is complete

    ![](part4_images/ascreenshot.jpeg)

4. You should now see the DEM on your map and in your Layers panel.

    ![](part4_images/screenshot_1.webp)