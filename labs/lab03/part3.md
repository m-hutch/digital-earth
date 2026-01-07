---
layout: default
title: Creating a Highlight Map
description: learn how to create a map that highlights one element
permalink: /labs/lab03/part3
active: True
nav: False
multi: True
prev: part2
next: part4
---

# Creating a Highlight Map

1. Click the blank area at the bottom of the layer pane to deselect the counties layer.

    ![](part3_images/ascreenshot.jpeg)


2. Click "Add Group"

    ![](part3_images/ascreenshot_1.jpeg)


3. Double-click "group1" and change the name to **"Highlight Map"**

    ![](part3_images/ascreenshot_2.jpeg)


4. Right click the county layer and click **"Duplicate Layer"**

    ![](part3_images/ascreenshot_3.jpeg)


5. drag the copy of the county layer into your new group

    ![](part3_images/ascreenshot_4.jpeg)


6. Right click the copied layer and rename it to "highlight_counties"

    ![](part3_images/ascreenshot_5.jpeg)


7. Click "highlight_counties"

    ![](part3_images/ascreenshot_6.jpeg)


8. Use the check boxes next to each layer to unselect all the layers outside the Highlight Map group and check all the layers inside the group

    ![](part3_images/ascreenshot_7.jpeg)


9. Double click the **highlight_counties** layer to open the properties. In the **Symbology** section, change the color to a neutral color (medium gray is best)

    ![](part3_images/ascreenshot_8.jpeg)


10. Click "Apply". You should be able to see the color you selected update on the map. Do not close the properties window.

    ![](part3_images/ascreenshot_9.jpeg)


11. Change "**Single Symbol**" to **"Rule-based"**

    ![](part3_images/ascreenshot_10.jpeg)


12. Click "Add rule"

    ![](part3_images/user_cropped_screenshot.png)


13. Click the build filter button

    ![](part3_images/user_cropped_screenshot_1.png)


14. Click the arrow next to "Fields and Values"

    ![](part3_images/ascreenshot_11.jpeg)


15. Double click "COUNTYFP"

    ![](part3_images/ascreenshot_12.jpeg)


16. Click "="

    ![](part3_images/ascreenshot_13.jpeg)


17. Type the county FP number you noted in the previous step. Dallas county's FP number is **113**, but you should type the FP number for your chosen county instead.

    ![](part3_images/ascreenshot_14.jpeg)


18. Click **OK**

    ![](part3_images/user_cropped_screenshot_2.png)


19. Click "Test"

    ![](part3_images/ascreenshot_15.jpeg)


20. Your filter should only return 1 feature. Click **OK** to close and **OK** again to close the filter menu

    ![](part3_images/user_cropped_screenshot_3.png)


21. Right click on your new rule and select **Change Color**

    ![](part3_images/ascreenshot_16.jpeg)


22. Choose a bright highlight color, then click **OK**

    ![](part3_images/ascreenshot_17.jpeg)


23. Click "Apply" then click "OK"

    ![](part3_images/ascreenshot_18.jpeg)


24. Your selected county should now be highlighted on the map

    ![](part3_images/user_cropped_screenshot_4.png)


25. Zoom out by scrolling to see the full state of Texas.

    ![](part3_images/user_cropped_screenshot_5.png)


