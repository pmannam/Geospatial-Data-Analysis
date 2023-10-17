# Spatial Analysis with SparkSQL

## Project Overview
In this project, we develop and execute various spatial queries on the database of a taxi cab firm, containing geographic and real-time location data of customers. To handle the large and mostly unstructured database, Big Data software application, SparkSQL is used. The primary objective of this project is to extract relevant data for both operational and strategic decision-making.

The project comprises two distinct phases. In the first phase, we will develop user-defined functions within SparkSQL to enable four spatial queries involving range, range join, distance, and distance join. The second phase focuses on 'hot zone analysis' and 'hot cell analysis,' involving spatial statistics to identify significant hot spots using Apache Spark.


## Phase 1: Spatial Queries

In this phase, we focus on implementing spatial queries using SparkSQL. These specialized queries work with geographic data and real-time location information. The goal is to efficiently extract relevant data from the large, unstructured database using SparkSQL, a popular Big Data software application.

### Key Objectives

1. **Range Query:**
   Find all points that fall within a given query rectangle (R) using the 'ST_Contains' function.

2. **Range Join Query:**
   Discover pairs of points and rectangles where a point is located within a specific rectangle using the 'ST_Contains' function.

3. **Distance Query:**
   Identify points lying within a specified distance (D) from a fixed point (P) using the 'ST_Within' function.

4. **Distance Join Query:**
   Determine pairs of points (p1, p2) where p1 is within a certain distance (D) from p2 using the 'ST_Within' function.

These queries are fundamental in spatial analysis and form the groundwork for the subsequent phase, where we delve into more complex spatial analysis tasks.


## Phase 2: Hot Spot Analysis
### 1. Hot Zone Analysis
- Perform a range join operation to calculate the hotness of rectangles based on the number of points they contain.

### 2. Hot Cell Analysis
- Implement spatial statistics to identify statistically significant spatial hot spots using the Getis-Ord statistic on NYC Taxi Trip datasets.

## Getting Started
To get started with this project, follow the steps outlined in each phase's respective folder. Make sure you have the necessary dependencies and data files available to run the code.

