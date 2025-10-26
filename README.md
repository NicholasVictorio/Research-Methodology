# 🗺️ Route Optimization in Kalimantan Barat using OR-Tools and Nearest Neighbor

This project demonstrates how to solve the **Traveling Salesman Problem (TSP)** for all regencies and cities (*kabupaten/kota*) in **Kalimantan Barat, Indonesia**.  
It compares the **Nearest Neighbor heuristic** and **Guided Local Search (GLS)** algorithm from **Google OR-Tools** using real-world road networks from **OpenStreetMap (OSM)** via **OSMnx**.

---

## 🚀 Features

- Fetches road network data for multiple cities in West Kalimantan using **OSMnx**
- Computes pairwise shortest path distances using **Dijkstra’s algorithm**
- Solves TSP using:
  - 🧭 **Nearest Neighbor (NN)** heuristic
  - 🧩 **Guided Local Search (GLS)** from Google OR-Tools
- Compares:
  - Total travel distance (km)
  - Execution time (seconds)
- Visualizes optimized routes using **matplotlib** and **OSMnx** map plotting

---

## 🧠 Algorithms

1. **Nearest Neighbor (NN)**  
   Greedy algorithm that selects the nearest unvisited city at each step.

2. **Guided Local Search (GLS)**  
   A metaheuristic from **Google OR-Tools** that iteratively improves the route by escaping local minima.

---

## 📦 Dependencies

Make sure to install the following Python packages:

```bash
pip install osmnx networkx numpy ortools matplotlib
