# Campus Navigation Bot 

![Python](https://img.shields.io/badge/Python-3.10-blue) ![License](https://img.shields.io/badge/License-MIT-green)

A **Jupyter Notebook project** that helps users navigate a campus efficiently using **reinforcement learning** algorithms like Q-Learning, SARSA, and Monte Carlo. This bot finds the **shortest and optimal paths** between locations on a campus map.

---

## Table of Contents
1. [Project Overview](#project-overview)  
2. [Features](#features)  
3. [Technologies Used](#technologies-used)  
4. [Installation](#installation)  
5. [Usage](#usage)  
6. [Results & Visualization](#results--visualization)  
7. [Future Improvements](#future-improvements)  
8. [License](#license)  

---

## Project Overview
The **Campus Navigation Bot** simulates navigation in a campus environment.  
It leverages **reinforcement learning** to find optimal paths between starting and goal points.  

Key points:  
- Supports multiple algorithms: **Q-Learning**, **SARSA**, and **Monte Carlo Control**.  
- Visualizes the path and value function using **matplotlib** and **seaborn**.  
- Calculates the **cost** and **steps** for each path.  

---

## Features
- Interactive Jupyter Notebook with organized code cells.  
- Automatic calculation of **optimal paths**.  
- Visualizations of:  
  - Path on campus map 🡆  
  - State value heatmaps  
  - Algorithm comparison for cost and steps  

---

## Technologies Used
- **Python 3.x**  
- **Jupyter Notebook**  
- **NumPy**  
- **Matplotlib**  
- **Seaborn**  

---

## Installation
1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/Campus-Navigation-Bot.git
2. Navigate to the project folder:

cd Campus-Navigation-Bot


3. Install dependencies:

pip install numpy matplotlib seaborn


4. Open the Jupyter Notebook:

jupyter notebook

Usage
Open Campus Navigation Bot.ipynb in Jupyter Notebook.
Run the cells sequentially.
Modify START and GOAL points to find paths between different locations.
Visualizations will display automatically for each algorithm.

Results & Visualization
Optimal path visualization using arrows 🡆
Heatmaps for state values of Q-Learning, SARSA, and Monte Carlo
Cost and steps comparison

Example Screenshots:




(Replace above paths with your actual screenshot images)

Future Improvements
Add a GUI interface for interactive campus navigation.
Include real campus map input with more complex routes.
Integrate user feedback for dynamic path updates.
Add more reinforcement learning algorithms for comparison.

License

This project is licensed under the MIT License – see the LICENSE
 file for details.

