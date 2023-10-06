---
layout: post
title: Troubleshooting pixelated images in a PDF exported from InDesign
category: Troubleshooting Article
permalink: /troubleshooting/
tags: user-documentation troubleshooting

---



## Problem

After exporting a PDF from InDesign, images are pixelated in the PDF, but not InDesign.


## Solution


### Check the format of the images in the InDesign file



1. Open the InDesign project file and find an image that looks pixelated in the exported PDF. **Click** on the image in the InDesign file.
2. In the menu bar, select **Window** > **Links.**
    * If some or none of the images in the **Links** panel end in _.svg_, follow the **[Relink high-quality images](#relink-high-quality-images)** instructions.
    * If all of the images in the **Links** panel end in _.svg_, follow the **[Adjust Performance Display settings](#adjust-performance-display-settings)** instructions.


### Relink high-quality images 

#### For macOS
<div class="code-example" markdown="1">
1. In the Links panel, select an image that does not end in _.svg_.
2. **Control-click** the image name and select **Reveal in Finder**.
3. In Finder, press **Command-3** to view as Columns. 
4. In the right column, scroll down and take note of the **Dimensions** and **Resolution**.
5. Look in the folder for other versions of the image. If there is a version that ends in _.svg_, then skip to Step 7. Otherwise, repeat Step 4 for each version of the image that you find. 
    * **Note:** Different versions of the same image should have the same name, but with different suffixes. For example, _leaf-1.png_, _leaf-2.png_, _leaf-3.jpg_ are different versions of the same image.
6. Identify the version of the image with the highest resolution and the largest dimensions.
7. Navigate back to InDesign and reopen the **Links** panel. **Control-click** on the highlighted image, click **Relink**, select the name of the version that ends in _.svg_ or that you identified in Step 6, and press **Open**.
8. Repeat Steps 1–7 for each image that looks pixelated in the exported PDF.
</DIV>

#### For Windows
<div class="code-example" markdown="1">
1. In the Links panel, select an image that does not end in _.svg_.
2. **Right-click** the image name and select **Reveal in Explorer**.
3. In Explorer, press **Alt + Enter** to open the properties window. 
4. Take note of the **Dimensions** and **Resolution**.
5. Look in the folder for other versions of the image. If there is a version that ends in _.svg_, then skip to Step 7. Otherwise, repeat Step 4 for each version of the image that you find. 
    * **Note:** Different versions of the same image should have the same name, but with different suffixes. For example, _leaf-1.png_, _leaf-2.png_, _leaf-3.jpg_ are different versions of the same image.
6. Identify the version of the image with the highest resolution and the largest dimensions.
7. Navigate back to InDesign and reopen the **Links** panel. **Right-click** on the highlighted image, click **Relink**, select the name of the version that ends in _.svg_ or that you identified in Step 6, and press **Open.**
8. Repeat Steps 1–7 for each image that looks pixelated in the exported PDF.
</div>

### Adjust Performance Display settings

1. In the menu bar, select **InDesign > Preferences > Display Performance**
2. Adjust the settings to match the following:
    * **Default View:** High Quality
    * **Preserve Object-Level Display Settings** is unchecked
    * **Adjust View Settings:** High Quality
    * **Raster Images:** High Resolution
    * **Vector Graphics:** High Resolution
    * **Transparency:** High Quality
    * **Enable Anti-aliasing** is checked
    * **Greek Type Below:** 7 pt
3. Click **OK**.

Now you can export the project as a PDF and the images will no longer be pixelated.

