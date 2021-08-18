---
title: Getting started
nav_order: 3
---

# Getting Started
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Creating a chart with Graph

In order to introduce you to our graphing tool, we will demostrate how to create charts using the Graph's interface to visualize SDDP case outputs. For the example, example case 20 will be used. It consists, basically, of one system containing three thermal plants supplying energy to consumers. Twelve stages constitute the study horizon, and the execution is deterministic.

For our first chart, let us suppose we are interested in visualizing the generations of each thermal plant in the system. So, to create the chart that fulfills out needs, follow the steps showed bellow. 

![](gifs/CreateChart_v2.gif)

The steps are listed below:

 1. Open Graph's interface
 2. Select the option to add new chart
 3. Choose the variable to be analyzed
 4. Configure the chart


## Using PSRIO to make custom charts

Now, let us make some processing over the standard output data using PSRIO. In the previous section, we created a chart with 3 curves, each one describing the generation of each thermal plant of system during the study period. Suppose that we want the aggregated thermal generation, which is not standard, instead of each one separately. We will use PSRIO to make this processing and create a new variable for us, so that we can plot it and analyze the result.

![](gifs/UsingPSRIOGraphIHM.gif)


The steps are listed below:

 1. Open PSRIO editor
 2. Write the script for the processing
 3. Select "Add chart" option
 4. Find your custom variable
 5. Configure and finish the chart

The recipe used for this example is the following:
```lua 
-- PSR Energy Consulting and Analytics
-- Graph 
-- Tutorial - Getting Started

-- load thermal collections and thermal generation data
thermal = require("collection/thermal");
gerter = thermal:load("gerter");

-- aggregate agents generations by sum and save to output file
total_gerter = gerter:aggregate_agents(BY_SUM(), "Total thermal");
total_gerter:save("total_gerter", {csv=true});
```



