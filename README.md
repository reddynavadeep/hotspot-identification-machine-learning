# machine-learning-hotspot-identification

##  Overview
Over the past couple of years, Indian Railways faced a deterioration of 5.30 percent in maintaining the punctuality of trains. Finding similar delay patterns across various stations where frequent delays occur, by trains passing through them and projecting the analysis results i.e., patterns on Maps, is the main objective. In this project, the region is restricted to Tamil Nadu and Kerala. The data collected is processed and clustering is done to obtain Dendograms to be projected. The latitude and longitude data of stations are gathered and the delay patterns i.e., Dendograms with various colour representations,. are plotted on Maps.

## Proposed System

1. Data gathering of delay schedules and official schedules of the trains considered from the official railway websites for analysis.
2. Data filtering based upon the scope of the project i.e., stations selected in the region of Tamil Nadu and Kerala part of the country.
3. Preprocessing raw data to formulate the links for the edges between all the stations along with the delay and actual arrival time at the stations.
4. Discretization of station link data points projected on time-delay matrix for simpler calculations.
5. Formulation of cost of transforming one edge to another using EMD Algorithm and computing distance matrix.
6. Distance matrix is given as input for Agglomerative clustering and six different clusters are obtained consisting of similar delay patterns.
7. The cluster data along with the latitude longitude data of stations is provided to the Tableau Data Visualization Tool and the patterns are generated on the Map.


## Methodology
The raw data, which includes train delays across various stations, is preprocessed and transformed into a format of links representing edges between consecutive stations. The data is then represented as a two-dimensional matrix, considering both the delay change value and the time it occurred. The density of delay changes is taken into account to handle variations in traffic. This also explains the process of delay change distribution representation and normalization.

## Implementation
It begins with data preprocessing, where the raw data is filtered based on official schedules and running schedules of the trains. The filtered data is used to create links between successive stations. A two-dimensional grid matrix is generated to represent the connected station edges. The section further explains the steps of representing data points in a matrix, normalization, agglomerative clustering, and the distance metric used for comparing edges. It concludes with the plotting of clusters on a map using Tableau data visualization tool.

## Results and Discussion
It includes visualizations of delay patterns in the states of Tamil Nadu and Kerala. Dual axis maps are used to map the edges and stations, and the links are categorized into clusters. The cluster-wise representation facilitates the analysis of similar delay patterns and their corresponding stations.
