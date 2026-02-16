# TSP Implementation

This repository focuses on solving the **Traveling Salesman Problem (TSP)** using various algorithms, including implementations for both theoretical graphs and a real-world application.

## Overview

The project contains two main implementations:

### 1. `tsp.ipynb` - Algorithm Comparison

Implementation and comparison of search algorithms for TSP:

- **UCS (Uniform Cost Search)** - Uninformed search algorithm
- **A\* with Nearest Edge Heuristic** - Informed search using minimum edge cost
- **A\* with MST Heuristic** - Informed search using Minimum Spanning Tree

Tested on a fully connected, symmetric, metric graph with 15 nodes. Includes performance analysis comparing cost and execution time.

### 2. `tsp-bc.ipynb` - Baja California Real-World Case

Real-world TSP implementation for Baja California:

- Creates a graph representing cities in Baja California
- Implements and compares advanced algorithms:
  - Lin-Kernighan (LKH)
  - Concorde Solver
  - Christofides Algorithm
  - Ant Colony Optimization (ACO)

## Usage

```bash
jupyter notebook tsp.ipynb
jupyter notebook tsp-bc.ipynb
```

## Key Features

- Exact algorithms for optimal solutions (UCS, A\*)
- Heuristic-based approaches for improved performance
- Real-world application with geographic data
- Performance benchmarking and algorithm comparison
