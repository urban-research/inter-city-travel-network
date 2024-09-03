# Inter-City Travel Network in South Korea

## Overview
This repository provides a visualization and analysis of the long-term evolution of inter-city travel networks in South Korea, covering the period from 1977 to 2016. By examining 40 years of data from both railway and highway travel networks, we explore the changing dynamics of inter-city connections and their implications for urban development.

The study investigates how the relationships between cities have evolved over time, focusing on key metrics such as traffic volume, network connectivity, and the emergence of hub cities. This analysis contributes to understanding the broader trends in urbanization and regional development in South Korea.

For a more detailed exploration of the data and results, please visit our [visualization dashboard](http://urban-research.github.io/inter-city-travel-network).

## Data Description

### Data Sources
- **Highway Travel Data:** Collected from the Korea Expressway Corporation's Toll Collection System (TCS). The data includes origin-destination information for all vehicles using South Korea's highways, recorded from 1977 to 2016. The TCS data provides comprehensive coverage of highway travel, including the number of trips between tollgates.
- **Railway Travel Data:** Sourced from annual reports published by the Korea Railroad Corporation (Korail). The data includes passenger trips between railway stations, based on ticket sales, from 1977 to 2016. This dataset reflects long-distance travel patterns across the country.

### Data Specifications
- **Temporal Coverage:** 1977-2016
- **Geographical Scope:** Includes 161 cities (nodes) in South Korea, categorized by administrative boundaries as of 2024. This includes six metropolitan cities (Daejeon, Daegu, Busan, Gwangju, Ulsan, Incheon) and the capital city (Seoul).
- **Data Format:**
  - **Highway Data:** Aggregated by city, representing annual travel volumes between pairs of cities.
  - **Railway Data:** Similarly aggregated by city, with travel volumes based on the number of trips between railway stations.
- **Exclusions:** Air traffic data is not included due to its negligible share (0.1%) of total inter-city transportation in South Korea.

### Methodology
- **Network Construction:** The travel networks are constructed as weighted networks, where nodes represent cities and edges represent the annual travel volumes between these cities. Nodes are included in the network if there is at least one recorded trip between them.
- **Analysis:** The study employs network science methods to analyze the structural properties of the travel networks, including metrics such as node degree, strength, and the rich-club effect. Scaling laws are also applied to examine the relationship between city population and travel volume.

## Repository Structure
- `data/`: Contains the raw and processed data files used in the analysis.
- `README.md`: This file.
- `index.html`: The main page for the visualization dashboard.
