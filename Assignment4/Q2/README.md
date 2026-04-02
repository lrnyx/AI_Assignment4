# Telangana Map Coloring using CSP (Automated Border Detection)

## Overview
This project solves the Map Coloring Problem for Telangana districts using Constraint Satisfaction Problem (CSP) techniques. It automatically detects neighboring districts from a KML map file and assigns colors such that no two adjacent districts share the same color.

---

## Key Features

- Automatic adjacency detection using geospatial data
- CSP-based map coloring using backtracking
- Heuristic optimization (most constrained district first)
- Randomized color selection for varied outputs
- Visualization using GeoPandas and Matplotlib

---

## Concepts Used

- Constraint Satisfaction Problem (CSP)
- Backtracking Algorithm
- Graph Coloring
- Heuristics (Degree Heuristic)
- Geospatial Data Processing

---

## Input

- A KML file (`telangana.kml`) containing district boundaries

---

## How It Works

1. Load the Telangana map using GeoPandas  
2. Detect neighboring districts using `.touches()`  
3. Build an adjacency graph  
4. Apply CSP with:
   - Backtracking
   - Degree heuristic (choosing most constrained district first)
5. Assign colors ensuring no adjacent districts match  
6. Plot the colored map  

---

## 🎨 Colors Used

- Red  
- Green  
- Blue  
- Yellow  

---

## Output

- A colored Telangana map where:
  - No adjacent districts have the same color
  - District names are labeled
  - Borders are clearly visible

---

