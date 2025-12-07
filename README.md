# Knapsack Genetic Algorithm 🎒🧬

**Classic 0/1 Knapsack optimization using genetic algorithm.** This project solves the famous combinatorial optimization problem by maximizing value under a strict weight constraint.

## 📋 Features
- **CSV Input:** Loads items (name, weight, value) dynamically from a CSV file
- **Genetic Algorithm:**
  - Population Size: 100
  - Generations: 100
  - Operators: Crossover + Mutation
- **Fitness Function:** Maximizes total value while penalizing solutions that exceed `max_weight`
- **CLI Interface:** Interactive max_weight setting → outputs optimal item selection

## 🛠️ Tech Stack
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)

## 🚀 Quick Start

**1. Prepare Data**
Create a CSV file (e.g., `items.csv`) with the format: `name,weight,value`
```text
Laptop,5,1000
Book,1,50
Phone,2,800
```

**2. Run the Solver**
```bash
python knapsack_ga.py
```

**3. Interact**
Enter your maximum weight capacity (e.g., `10`) when prompted to see the optimal combination.

## 🧬 Algorithm Flow

```text
Population (100) → Fitness Evaluation → Selection → Crossover → Mutation (10%)
       ↑                                                           |
       └────────────────── Repeat 100 Generations ◄────────────────┘
                                     ↓
                              Best Solution Found
```

## 🎯 Example Scenario

```text
Max Weight: 10

Input Items:
- Laptop (Weight: 5, Value: 1000)
- Book   (Weight: 1, Value: 50)
- Phone  (Weight: 2, Value: 800)

Output:
[Laptop, Phone]
Total Value: 1800
Total Weight: 7
```

## 📁 Files
```text
├── knapsack_ga.py         # Complete GA implementation
└── sample_items.csv       # Example input (not included)
```
