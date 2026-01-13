---
layout: default
title: Making a Hillshade
description: ...
permalink: /labs/lab05/part5
active: True
nav: False
multi: True
prev: part4
next: part6
---

# How to create a hillshade image from a DEM

1. Click **Raster &gt; Analysis &gt; "Hillshade…"**

    ![](part5_images/screenshot.webp)


2. In the Raster Analysis window, make sure your **DEM** is selected as the Input layer.

    Set the **Z factor** to 0.00004

    The **Azimuth** and **Altitude** settings control where the simulated sun would appear in the sky. You can adjust these settings to change the time of day and affect how the shadows appear on the terrain. for now, leave them at their default values.

    ![](part5_images/user_cropped_screenshot.png)


3. Scroll down in the Raster Analysis window and use the three dots "..." to select a file location to save the Hillshade layer.

    Save the image under the name **hillshade.tif** in your Lab 5 folder.

    ![](part5_images/screenshot_1.webp)


4. Make sure the **Open output file** option is checked.

    Click **"Run"**

    ![](part5_images/user_cropped_screenshot_1.png)


5. Once the calculation in finished, click **close** to close the Raster Analysis window.


6. Your hillshade layer should now be visible on the Map.

    ![](part5_images/screenshot_2.webp)