# K-Means Constrained Clustering for 7/11 Stores

## Overview
This project clusters multiple 7/11 store locations using the `k-means-constrained` algorithm. After fetching the addresses, they are geocoded to obtain longitude and latitude details. These positions are processed and converted into Cartesian coordinates. The main goal is to cluster the stores and find the optimal route for each 7/11 cluster using the Traveling Salesman Problem (TSP).

## Installation
To use this project, the following packages need to be installed:

pip install k-means-constrained


## Project Structure

1. **Data Sources**:
    - 7/11 store locations: [source](https://www.ibon.com.tw/retail_inquiry.aspx#gsc.tab=0)
    - Taiwan Town and City Area Boundaries: [source](https://sheethub.com/ronnywang/%E9%84%89%E9%8E%AE%E5%B8%82%E5%8D%80%E8%A1%8C%E6%94%BF%E5%8D%80%E5%9F%9F%E7%95%8C%E7%B7%9A/uri/19260536)
    - k-means-constrained GitHub repository: [source](https://github.com/joshlk/k-means-constrained)

2. **Main Process**:
    - Read and process the 7/11 store location data from `711_data.csv`.
    - Convert longitude and latitude data into Cartesian coordinates.
    - Cluster the 7/11 store locations using `KMeansConstrained`.
    - Apply the Traveling Salesman Problem (TSP) on each cluster to determine the optimal route for visiting each 7/11 store within a cluster.

3. **Output**:
    - The optimal route for each cluster of 7/11 stores.
    - The total distance required to traverse each cluster using the optimal route.

## Usage

1. Prepare the data by fetching 7/11 addresses and geocoding them using Google Sheets with the `geocoding by smartmokey` extension.
2. Import the processed data as a CSV file into the code.
3. Run the provided code to cluster the 7/11 store locations.
4. Apply the TSP algorithm to determine the optimal route for visiting each store within each cluster.
5. Review the output to get the optimal route and total distance for each cluster.

## Credits

- The k-means-constrained algorithm is sourced from [this GitHub repository](https://github.com/joshlk/k-means-constrained).

