---
title: "Extracting the geographic features you need from a larger dataset in ArcGIS Pro"
layout: "home"
description: "You may have noticed that many GIS datasets contain information about a geographic extent that is larger than your area of interest. Your research may involve analysis of data related to a single municipality in Ontario, yet you have only been able to locate a dataset showing all municipalities located within the province. Alternatively, you may be interested in only displaying a selection of features on your completed map, such as the Canadian cities you have selected as case studies for your research. This tutorial will demonstrate how to extract just the features you need from larger datasets, saving them to new files that you can then use to map and analyze your data."
staff:
    - name: Nick Field
      link: https://library.utoronto.ca/staff/nick-field
maintainer: 
    - name: Cole White
      link: https://library.utoronto.ca/staff/cole-white 
created_date: 2024-02-06
permalink: "/"  #! Remove this if not the homepage
---

# Extracting the geographic features you need from a larger dataset in ArcGIS Pro

You may have noticed that many GIS datasets contain information about a geographic extent that is larger than your area of interest. Your research may involve analysis of data related to a single municipality in Ontario, yet you have only been able to locate a dataset showing all municipalities located within the province. Alternatively, you may be interested in only displaying a selection of features on your completed map, such as the Canadian cities you have selected as case studies for your research. This tutorial will demonstrate how to extract just the features you need from larger datasets, saving them to new files that you can then use to map and analyze your data.

1. Use the **Add Data** button to add the dataset you are interested in selecting from to your map document. For this example, we will use a shapefile that represents the dissemination areas that comprise the Toronto Census Subdivision (From Statistics Canada) to create a new dataset that depicts just the boundaries of High Park.

    <img src='{{ '/assets/images/1_1.png' | relative_url }}' alt='drop down menu after clicking the Add Data button' title='' width='395' height='827' />

2. Right-click on the name of the dataset in the Table of Contents, and select **Attribute Table**.

    <img src='{{ '/assets/images/2_0.png' | relative_url }}' alt='Pop up after right clicking the feature layer with attribute table highlighted' title='' width='441' height='778' />

3. Click in the grey box to the left of the row in which High Park appears. The row will be highlighted in blue. (If you were looking to select multiple, holding down the Ctrl key will allow you to select more than one at once.) The outline of the dissemination area will be highlighted in blue.

    <img src='{{ '/assets/images/3_0.png' | relative_url }}' alt='Attribute table with a row highlighted and the dissemination area boundaries around High Park outlined in light blue' title='' width='807' height='479' />

4. Right-click on the name of the layer in the Table of Contents, select **Data**, then **Export Features...**

    **<img src='{{ '/assets/images/4_0.png' | relative_url }}' alt='Popup menu after right clicking on the feature layer, Data, export features is highlighted' title='' width='605' height='770' />**

5. In the Export Features window that appears, the parameters are already selected (because we selected them in the previous step). Confirm that they are as wanted, if you wish to rename the exports output, do so now in the "Output Feature Class" text bar. Remember to keep the file extension as ".shp". Press OK to complete the export process.

    <img src='{{ '/assets/images/5_0.png' | relative_url }}' alt='Export features popup with the input and output features input' title='' width='400' height='285' />

    The exported layer will appear on top (higher in the draw order), you can disable or delete the old layer if wanted.
6. Alternatively, you can use the different Select tools instead of selecting rows from the attribute table to interactively select features from the map.

    <img src='{{ '/assets/images/6_0.png' | relative_url }}' alt='pop up from the Selection category, showcasing the different ways of selecting shape files' title='' width='204' height='470' />

Technique: [Extracting data](https://mdl.library.utoronto.ca/technique/extracting-data) | Tools: [ArcGIS Pro](https://mdl.library.utoronto.ca/taxonomy/term/70) | Data Format: [Vector](https://mdl.library.utoronto.ca/data-format/vector)
