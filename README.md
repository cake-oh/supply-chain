# Supply Chain Analysis

This repository stores data and code for an analysis of fishing vessel movements. The driving question is *"How are harvesting and landing sites in the Western Central Pacific Ocean changing, and what are the drivers?"*

**Overall Approach:**
1. Run a spatial clustering analysis of vessel movements to calculate Harvesting and Landing Sites
2. Create Harvest-to-Landing Networks and analyze topology 
3. Run a longitudinal/predictive network analysis (i.e., ERGM)

## Step 1
This step is to analyze vessel movement data from 2017 to 2021 using Global Fishing Watch's [Apparent Fishing Effort Dataset](https://globalfishingwatch.org/dataset-and-code-fishing-effort/) based on Automatic Identification System (AIS) data.

*Q's to resolve:* Which vessels to look at? Use all over the entire area, or divide by fleet/gear type?

## Step 2
The derived locations from Step 1 will be used to create Harvest-to-Landing Networks, where nodes are Harvest or Landing Sites connected by edges weighted by the amount of vessels flowing between these locations. Network analysis will assess the network's topology (e.g., density, richness, modularity, centralization).

*Q's to resolve:* Any other network metrics to include?

## Step 3
These networks will be enhanced with additional data characterizing the flag nations (nodes) represented in the fishing fleets. National variables like GDP, seafood demand, fisheries subsidies, etc.

*Q's to resolve:* What are other interesting variables? Is it possible to run an analysis including "general" variables that are not country-specific, such as sea surface temperature or fuel prices?
