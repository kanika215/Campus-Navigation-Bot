# 📌 Campus Navigation Project

Reinforcement Learning–based grid navigation system implemented on a **5×5 campus layout**.  
The agent learns to move from **Hostel (Start)** to **Library (Goal)** while avoiding obstacles.

This project implements and compares four RL algorithms:

- **Q-Learning**
- **SARSA**
- **Monte Carlo Control**
- **Temporal Difference (TD-λ)**

All code is implemented inside:

📄 **Campus Navigation Bot.ipynb**

---

## 📑 Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [File Structure](#file-structure)
- [How to Run](#how-to-run)
- [Campus Environment](#campus-environment)
- [Algorithms Implemented](#algorithms-implemented)
  - [Q-Learning](#1️⃣-q-learning)
  - [SARSA](#2️⃣-sarsa)
  - [Monte Carlo Control](#3️⃣-monte-carlo-control)
  - [Temporal Difference (TD-λ)](#4️⃣-temporal-difference-td-λ)
- [Output Visualizations](#output-visualizations)
- [Use Cases](#use-cases)
- [Requirements](#requirements)


---

## 🏫 **Project Overview**
This project simulates a **campus navigation environment** represented as a 5×5 grid.  
Each grid cell corresponds to a real-world campus location such as:

- Hostel (Start)
- Walkways
- Admin Buildings (Obstacle)
- Park (Obstacle)
- Sports Complex (Obstacle)
- Library (Goal)

The goal of the agent is to learn the **optimal path** using different Reinforcement Learning algorithms.

---

## ✨ **Features**
- ✔ Custom 5×5 campus grid  
- ✔ Four RL algorithms  
- ✔ Arrow-based navigation path visualization  
- ✔ Reward vs Episode learning curves  
- ✔ Q-Table generation  
- ✔ Same environment for all algorithms  
- ✔ Clean, modular code  

---

## 📁 **File Structure**

```
Campus Navigation Bot.ipynb  
README.md
```

Notebook includes:

- Environment setup  
- Rewards  
- Step function  
- Visualization functions  
- Q-Learning / SARSA  
- Monte Carlo Control  
- TD-λ  
- Final outputs  

---

## ▶️ **How to Run**

### **1️⃣ Install Dependencies**
```bash
pip install numpy matplotlib
```

### **2️⃣ Run the Notebook**
Open `Campus Navigation Bot.ipynb` in:

- Jupyter Notebook  
- OR VS Code (with Jupyter extension)

Run all cells to see outputs.

---

## 🗺 **Campus Environment**

The campus is a 5×5 grid with rewards:

| Location | Reward |
|---------|--------|
| Walkway | -1 |
| Admin / Park / Sports Complex (Obstacles) | -5 |
| Goal (Library) | +10 |
| Invalid Move | Penalty |

Obstacles block movement.

---

# 🔍 **Algorithms Implemented**

## 1️⃣ Q-Learning
**Off-policy TD control**  
Update rule:
```
Q[s][a] = Q[s][a] + α * (r + γ * max(Q[s']) - Q[s][a])
```

Outputs:
- Q-table  
- Optimal path  
- Reward curve  

---

## 2️⃣ SARSA
**On-policy TD control**  
Update rule:
```
Q[s][a] = Q[s][a] + α * (r + γ * Q[s’][a’] - Q[s][a])
```

Outputs:
- Q-table  
- Optimal path  
- Reward graph  

---

## 3️⃣ Monte Carlo Control
Episode-based learning.  
Updates occur after each episode.

Outputs:
- Path  
- Costs  
- Reward curves  

---

## 4️⃣ Temporal Difference (TD-λ)
Uses **eligibility traces**, faster convergence.

Outputs:
- Path  
- Costs  
- Learning curve  

---

## 📊 **Output Visualizations**
The notebook produces:

- 📈 Reward vs Episodes  
- 🧭 Arrow-based optimal path  
- 🟩 Campus grid  
- 🧮 Q-Tables  
- 🔄 Algorithm comparisons  

---

## 🧠 **Use Cases**
Useful for:

- RL learning  
- Gridworld experiments  
- University projects  
- Navigation simulations  
- Algorithm comparison studies  

---

## 🛠 **Requirements**
- Python 3.8+  
- numpy  
- matplotlib  

---

If you want a **project banner**, **badges**, or **GIF of path animation**, tell me! 🚀
