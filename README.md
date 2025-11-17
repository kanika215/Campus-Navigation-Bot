# 🎓 Campus Navigation Project

Reinforcement Learning–based grid navigation system implemented on a 5×5 campus layout.  
The agent learns to move from Hostel (Start) to Library (Goal) while avoiding obstacles.

This project implements and compares four RL algorithms:

- Q-Learning  
- SARSA  
- Monte Carlo Control  
- Temporal Difference (TD-λ)

All code is implemented in:

📄 **Campus Navigation Bot.ipynb**

---

## 📑 Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [File Structure](#file-structure)
- [How to Run](#how-to-run)
- [Campus Environment](#campus-environment)
- [Algorithms Implemented](#algorithms-implemented)
  - [Q-Learning](#q-learning)
  - [SARSA](#sarsa)
  - [Monte Carlo Control](#monte-carlo-control)
  - [Temporal Difference (TD-λ)](#temporal-difference-td-λ)
- [Output Visualizations](#output-visualizations)
- [Use Cases](#use-cases)
- [Requirements](#requirements)

---

## Project Overview

The environment is a 5×5 grid representing a campus map.  
Each cell corresponds to a location such as:

- Hostel  
- Walkways  
- Admin Building (Obstacle)  
- Park (Obstacle)  
- Sports Complex (Obstacle)  
- Library (Goal)

The agent receives rewards based on movement, collisions, and reaching the goal.

This project showcases how four RL algorithms learn optimal navigation paths on the **same campus layout**.

---

## Features

✔ Custom 5×5 campus environment  
✔ Four RL algorithms implemented from scratch  
✔ Arrow-based path visualization  
✔ Campus grid with labeled buildings  
✔ Reward trend graphs  
✔ Q-table outputs (Q-Learning & SARSA)  
✔ Full comparison of algorithm behavior

---

## File Structure

```
Campus Navigation Bot.ipynb   → Complete implementation
README.md                     → Project documentation
```

Contents inside the notebook:

- Environment setup (grid, labels, obstacles, movement rewards)
- Q-Learning  
- SARSA  
- Monte Carlo Control  
- Temporal Difference (TD-λ)  
- Visualization utilities

---

## How to Run

### Step 1: Install dependencies
```bash
pip install numpy matplotlib
```

### Step 2: Execute the notebook
Run:

```
Campus Navigation Bot.ipynb
```

The notebook will:

- Train all RL algorithms
- Display reward graphs
- Visualize optimal navigation paths
- Print Q-tables (Q-Learning, SARSA)

---

## Campus Environment

Reward structure:

| Location Type | Reward |
|--------------|--------|
| Walkway | -1 |
| Obstacles (Admin, Park, Sports) | -5 |
| Goal (Library) | +10 |
| Invalid Move | Penalty |

The grid is fully labeled and visualized.

---

## Algorithms Implemented

### Q-Learning
Off-policy TD control method  
Update rule:

```
Q[s][a] = Q[s][a] + α * (r + γ * max(Q[s’]) - Q[s][a])
```

Outputs:
- Q-Table  
- Total cost  
- Optimal path  
- Reward graph  

---

### SARSA
On-policy TD control method  
Update rule:

```
Q[s][a] = Q[s][a] + α * (r + γ * Q[s’][a’] - Q[s][a])
```

Outputs:
- Q-Table  
- Total cost  
- Optimal path  
- Reward graph  

---

### Monte Carlo Control

Learns action-values using full-episode returns.  
No bootstrapping.

Outputs:
- Optimal path  
- Total cost  
- Reward graph

---

### Temporal Difference (TD-λ)

Combines TD learning with eligibility traces.  
More efficient propagation of reward information.

Outputs:
- Optimal path  
- Total cost  
- Reward graph

---

## Output Visualizations

The project automatically generates:

- Reward curves for all algorithms  
- Grid-based path visualizations  
- Arrow-based movement paths  
- Q-tables  
- Final optimal policies  

---

## Use Cases

This project is ideal for:

- RL learning and comparison  
- University projects  
- Research demonstrations  
- Understanding convergence behavior  
- Pathfinding and navigation systems  

---

## Requirements

- Python 3.8+
- numpy
- matplotlib


