---
title: "Extracting the geographic features you need from a larger dataset in ArcGIS Pro"
layout: "home"
description: "You may have noticed that many GIS datasets contain information about a geographic extent that is larger than your area of interest. Your research may involve analysis of data related to a single municipality in Ontario, yet you have only been able to locate a dataset showing all municipalities located within the province. Alternatively, you may be interested in only displaying a selection of features on your completed map, such as the Canadian cities you have selected as case studies for your research. This tutorial will demonstrate how to extract just the features you need from larger datasets, saving them to new files that you can then use to map and analyze your data."
staff:
    - name: Nick Field
      link: https://library.utoronto.ca/staff/nick-field
    - name: Cole White
      link: https://library.utoronto.ca/staff/cole-white 
maintainer: 
    - name: Cole White
      link: https://library.utoronto.ca/staff/cole-white 
created_date: 2024-02-06
permalink: "/"  #! Remove this if not the homepage
---

# Extracting the geographic features you need from a larger dataset in ArcGIS Pro

You may have noticed that many GIS datasets contain information about a
<b>geographic extent that is larger than your area of interest</b>.

<b>Example:</b> This Statistics Canada layer (downloaded from
<a href="https://www12.statcan.gc.ca/census-recensement/2021/geo/sip-pis/boundary-limites/index2021-eng.cfm?year=21"
target="_blank">this page</a>), displays all census dissemination areas within
Canada. Suppose you only need to work with (for example) Nova
Scotia's dissemination areas. This tutorial will demonstrate
how to extract just the features you need, saving them to
new files that you can then use to map and analyze your data.

<a href='{{ '/assets/images/lda.png' | relative_url }}' target="_blank">
<img src='{{ '/assets/images/lda.png' | relative_url }}' alt="Canada
census dissemination area polygons" width='100%' height='100%'  style="border:
3px solid #888888;" />
</a>

### Selecting a subset by attributes

• Open the layer's <b>attribute table</b> by right-clicking on
it in the Contents pane and choosing <b>Attribute table</b>.

<a href='{{ '/assets/images/show-attribute-table.png' | relative_url }}' target="_blank">
<img src='{{ '/assets/images/show-attribute-table.png' | relative_url }}' alt="
Show the attribute table" width='70%' style="border: 3px solid #888888;" />
</a>

• Click <b>Select by attributes</b>

<a href='{{ '/assets/images/select-by-attributes.png' | relative_url }}' target="_blank">
<img src='{{ '/assets/images/select-by-attributes.png' | relative_url }}' alt="
Select by attributes" width='100%' height='100%' style="border: 3px solid #888888;" />
</a>

• Query the relevant features. Click <b>OK</b>. The features will be selected.
In this example, features have been queried according to a categorical value
(PRUID 12 means Nova Scotia in this dataset). You might also try querying
features by size - for example, maybe you're only interested in polygons above
or below a particular area threshold, or lines within a certain distance range.

<a href='{{ '/assets/images/query-features.png' | relative_url }}' target="_blank">
<img src='{{ '/assets/images/query-features.png' | relative_url }}' alt="
Query data" width='70%' style="border: 3px solid #888888;" />
</a>

• Right-click the layer name in the Contents pane. Choose <b>Data -> Export
features</b>.

<a href='{{ '/assets/images/data-export-features.png' | relative_url }}' target="_blank">
<img src='{{ '/assets/images/data-export-features.png' | relative_url }}' alt="
Data -> Export features" width='100%' height='100%' style="border: 3px solid #888888;" />
</a>

• Make sure that the <b>Use the selected records</b> option is toggled on, and click
<b>OK</b>.

<a href='{{ '/assets/images/use-selected-records.png' | relative_url }}' target="_blank">
<img src='{{ '/assets/images/use-selected-records.png' | relative_url }}' alt="
Use the selected records" width='70%' style="border: 3px solid #888888;" />
</a>

• This will result in a new layer containing only the previously selected
features. It can now be added to ArcGIS Online.

<a href='{{ '/assets/images/subsetted-layer.png' | relative_url }}' target="_blank">
<img src='{{ '/assets/images/subsetted-layer.png' | relative_url }}' alt="
New subset layer" width='100%' height='100%' style="border: 3px solid #888888;" />
</a>

### Selecting data interactively from the Attribute Table or the map

• Right-click on the name of the dataset in the Table of Contents, and
select **Attribute Table**.

<img src='{{ '/assets/images/2_0.png' | relative_url }}'
alt='Pop up after right clicking the feature layer with attribute table highlighted'
title='' width='441' height='778' />

• Click in the <b>grey box</b> to the left of your feature of interest (High
Park, Toronto, in this example).
The row will be highlighted in blue. (If you were looking to select multiple,
holding down the Ctrl key will allow you to select more than one at once.) The
outline of the dissemination area will also be highlighted in blue.

<img src='{{ '/assets/images/3_0.png' | relative_url }}'
alt='Attribute table with a row highlighted and the dissemination area
boundaries around High Park outlined in light blue' title=''
width='807' height='479' />

• Right-click on the name of the layer in the Table of Contents, select
**Data**, then **Export Features...**

**<img src='{{ '/assets/images/4_0.png' | relative_url }}'
alt='Popup menu after right clicking on the feature layer, Data, export
features is highlighted' title='' width='605' height='770' />**

• In the Export Features window that appears, the parameters are already
selected (because we selected them in the previous step). Confirm that they are
as wanted, if you wish to rename the exports output, do so now in the
<b>Output Feature Class</b> text bar. Remember to keep the file extension as
'.shp'. Press <b>OK</b> to complete the export process.

<img src='{{ '/assets/images/5_0.png' | relative_url }}'
alt='Export features popup with the input and output features input'
title='' width='400' height='285' />

The exported layer will appear on top (higher in the draw order). You can
disable or remove the old layer if wanted.

• Alternatively, you can use the different <b>Select</b> tools instead of
selecting rows from the attribute table to interactively select features from
the map.

<img src='{{ '/assets/images/6_0.png' | relative_url }}'
alt='pop up from the Selection category, showcasing the different ways of selecting shape files'
title='' width='204' height='470' />

**Technique:** [Extracting data](https://mdlutoronto.github.io/tutorials-search/?technique=Extracting+data)\|
**Tools:** [ArcGIS Pro](https://mdlutoronto.github.io/tutorials-search/?tool=ArcGIS+Pro) \|
**Data Format:** [Vector](https://mdlutoronto.github.io/tutorials-search/?dataFormat=Vector)
