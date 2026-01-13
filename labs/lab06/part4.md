---
layout: default
title: Create Buffer Layer
description: Learn how to create a buffer around features
permalink: /labs/lab06/part4
active: True
nav: False
multi: True
prev: part3
next: part5
---

# How to Create Buffer Layer


1. Click **Vector &gt; Geoprocessing Tools &gt; Buffer…**

    ![](part4_images/screenshot.webp)


2. For **Input layer** select the **TR_sites_1mi_near_Dallas** layer

    For **Distance**, select **1 mile**

    ![](part4_images/user_cropped_screenshot.png)


3. Click **Run**. When the process is complete, click **Close**.


4. We now have a layer of 1-mile buffers around every TR site. Notice that by default, the buffer layer is a temporary layer. This means if you close QGIS, this layer will disappear.

    ![](part4_images/user_cropped_screenshot_1.png)


5. Examine the Attribute Table of our new **Buffered** layer. Notice that it is exactly the same as the original TRI_sites table.

