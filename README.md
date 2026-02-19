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

---

## 🛠️ Environment Setup

Follow these steps to ensure you are using the same library versions as the rest of the team.

### 1. Create the Virtual Environment

Open your terminal in the project root and run:

```bash
# Windows
python -m venv .venv

# macOS/Linux
python3 -m venv .venv
```

### 2. Activate the Environment

You should activate the environment before installing any packages.

```bash
# Windows (Command Prompt)
.venv\Scripts\activate

# Windows (PowerShell)
.\venv\Scripts\Activate.ps1

# macOS/Linux
source .venv/bin/activate
```

### 3. Install Dependencies

This will install all necessary libraries, including ipykernel which VS Code needs to run the notebooks.

```bash
pip install -r requirements.txt
```

## 📓 Running Notebooks in VS Code

1. Open a `.ipynb` file in VS Code.
2. Look at the top-right corner of the editor.
3. Click on **Select Kernel**.
4. Choose **Python Environments...** and select the one pointing to `./.venv/bin/python` (or `Scripts/python.exe` on Windows).

## 📦 Managing Dependencies

If you need to add a new library (e.g., pandas or matplotlib):

1. Activate your venv:
   ```bash
   # Windows
   .venv\Scripts\activate
   
   # macOS/Linux
   source .venv/bin/activate
   ```

2. Install the library:
   ```bash
   pip install <library-name>
   ```

3. Update the requirements file:
   ```bash
   pip freeze > requirements.txt
   ```

4. Commit the updated `requirements.txt` so the rest of the team can run `pip install -r requirements.txt` to sync up.
