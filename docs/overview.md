---
title: Overview
nav_order: 2
---

# Overview
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Opening Graph throught SDDP's interface

Graph's application can be opened via SDDP's interface. In the menu bar, search for its icon, as ilustrated below:

<div style="text-align:center">
    <img src="images\OpeningGraphSDDP_v2.png" width="600"/>
</div>

## Graph's interface main sections

After opening the interface, at first glance, it will be possible to see the following areas:

<div style="text-align:center">
    <img src="images\GraphIHM_v2.png" width="600"/>
</div>

Which are:

1. Menu pages
2. Chart options
3. Chart board


### Menu pages

In this part of the interface, it is possible to open PSRIO editor and the charts page.

See more of PSRIO at https://psrenergy.github.io/psrio-scripts/.
### Chart options

In chart options, it will be possible to:

* Add new charts to the dashboard
* Move the charts around the dashboard
* Update charts data
* Change theme and dashboard layout

Buttons for theme change e layout modification are, respectively, from left to right, the following:

<div style="text-align:center">
    <img src="images\ThemeLayoutButtons.png" width="100"/>
</div>

#### Adding new charts

To add a new chart, select the "Add chart" button located on the top right side of the interface. The following window will be opened:

<div style="text-align:center">
    <img src="images\AddChartWindow_v2.png" width="450"/>
</div>

On the top field, a name can be given to the chart. In the button "Variables", the variables to be displayed in the graph can be chosen. Selecting this, another window will be opened:

<div style="text-align:center">
    <img src="images\VariablesSelectionWindow_v2.png" width="450"/>
</div>

The list highlighted by the red box contains all the available variables that can be displayed in the chart. Select one of them. After doing so, the agents related to those variables will be shown in the table highlighted by the purple box, when the tab "Agents" is selected. If "Macro agents" is selected, the agents of the same type will be agregated into one, and it will be possible to plot agregated variables such as "TotalHydro" and "TotaTherm", for example, which represents total hydroelectric and thermal generations, respectively. After selecting the agents, hit the "Ok" button.

 The next step is to configure the horizon, blocks and scenarios of the data that will appear on the chart. The process of adding the new chart can be finished giving a good title to it. Following these steps, charts like this can be created:

 <div style="text-align:center">
    <img src="images\ChartExample.png" width="450"/>
</div>

### Chart board

The chart board is where the charts will be displayed and the user will be able to analyze the output of SDDP. Once the chart is created, it is possible to change its type, add or remove legends, configure the data, download or remove the chart.

#### Changing the chart's type and layout

Once the chart is created, select the button on the top left side of the chart's area:

<div style="text-align:center">
    <img src="images\ChangeChartTypeLayout.png" width="450"/>
</div>

In "Chart type" section, several types can be chosen. Choose what is best for you. In "Layout", the legends can be removed or introduced.

#### Configuring, downloading and removing charts

To download, configure or remove the chart, respectively, from left to right, go to the top right side of the chart:

<div style="text-align:center">
    <img src="images\ChartDownloadConfigDelete.png" width="450"/>
</div>

* Download button:
  
The download button will give two options, as ilustrated below:

<div style="text-align:center">
    <img src="images\DownloadOptions.png" width="200"/>
</div>

* Configuration button:
  
The configuration button will just reopen the same window used when chart was added for the first time. So it is possible to change the data displayed, after the creation of the chart.

* Delete button

The chart will be deleted from the chart board.


