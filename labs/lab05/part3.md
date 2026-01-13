---
layout: default
title: Capture Satellite Image
description: ...
permalink: /labs/lab05/part3
active: True
nav: False
multi: True
prev: part2
next: part4
---
# Capture a high-resolution Satellite Image

Before you start, make sure you have installed the required plugins:
- Lat Lon Tools
- OpenTopography DEM Downloader
- HCMGIS

1. Navigate to [https://earth.google.com](https://earth.google.com/web/) and click **Explore Earth**

    ![](part3_images/user_cropped_screenshot.webp)


2. Search for the name of the location you want to capture satellite imagery of

    ![](part3_images/ascreenshot.jpeg)


3. Right-click on the center of the location

    ![](part3_images/ascreenshot_1.jpeg)


4. **Copy coordinates**

    ![](part3_images/ascreenshot_2.jpeg)


5. In **QGIS**, create a new project and save it in your Lab 5 folder


6. Click **HCMGIS &gt; Basemaps &gt; Esri Imagery**

    ![](part3_images/user_cropped_screenshot_1.webp)


7. Click **Plugins &gt; Lat Lon Tools &gt; Zoom To Coordinate**

    ![](part3_images/screenshot.webp)


8. You should now have a Zoom to Coordinate pane in the bottom left corner. **Paste your point coordinates** from Google Earth, then click the **zoom to coordinate** button.

    ![](part3_images/user_cropped_screenshot_2.webp)


9. A red cross will appear over your point and will center your point on the map view. Change the **Scale** **to 1:30000** and press **enter/return** **key** on your keyboard

    ![](part3_images/user_cropped_screenshot_3.webp)


    <span class='tip'>You should now see your location in detail. Be careful not to zoom in more past this point. If you accidentally zoom in or out, you can reset to this view by changing the **Scale** back to 1:30000</span>

    ![](part3_images/user_cropped_screenshot_4.webp)


10. Find the UTM Zone that covers your point of interest. You can use a site like <https://utmzone.optimumgeospatial.co.ke/>

    ![](part3_images/user_cropped_screenshot_5.webp)


11. Click the "Current CRS" Button in the bottom right corner

    ![](part3_images/user_cropped_screenshot_6.webp)


12. In the **CRS** tab of the **Project Properties** window, search for the UTM zone that covers your area of interest and select it. Make sure that your point is visible inside the extent highlighted in red.

    ![](part3_images/user_cropped_screenshot_7.webp)


    <span class='alert'>Make sure you do step 12! If you skip it, you may not get any error warnings, but your final 3D view will render **extremely slowly.**</span>


13. Create a new print layout called **satellite_image**

    ![](part3_images/screenshot_1.webp)


14. Add a map to the page and adjust the edges to cover the entire page, with no margins.

    ![](part3_images/screenshot_2.webp)


15. Click **Export as image**

    ![](part3_images/user_cropped_screenshot_8.webp)


    <span class='tip'>Tip: If you get a warning about WMS layers, click **Close**.</span>


16. save the layout as a .TIF file in your Lab 5 folder

    ![](part3_images/screenshot_3.webp)


17. In the **Image Export Options** window, change the **Page width** to **16384 px**. The Export resolution and page height will update automatically (it's okay if they are slightly different numbers than the screenshot).

    Check the **Generate world file**.

    Click **Save**

    ![](part3_images/user_cropped_screenshot_9.webp)


    <span class='alert'>If you have an older computer, or if your computer is taking a long time to open the exported file, you can export the image at a lower resolution (8192px recommended). Keep in mind this may make your final 3D model look pixelated because it is a lower quality image. You will not loose points for this. </span>


18. If you saved the image in the same folder as your QGIS project, you can drag the image directly into your layer pane from the **Project Home Folder**.

    If you saved the image somewhere else, you can add the image by using the **Data Source Manager** and choosing the **Raster** tab, then select your image file to import and click **Add**.

    ![](part3_images/screenshot_4.webp)


19. Remove the Esri Imagery Layer

    ![](part3_images/screenshot_5.webp)


20. Close the Zoom to Coordinate window to remove the red cross from your map

    ![](part3_images/user_cropped_screenshot_10.webp)


    ![](part3_images/screenshot_6.webp)