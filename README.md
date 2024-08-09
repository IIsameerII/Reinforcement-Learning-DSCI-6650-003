# Reinforcement-Learning-DSCI-6650-003

This repository contains the code and analysis for computing value functions in a 7x7 gridworld environment using various reinforcement learning methods. The gridworld environment is used to illustrate the application of reinforcement learning techniques such as SARSA, Q-Learning, Gradient Monte Carlo, and Semi-gradient TD(0) with an affine function approximation.

## Project Structure

- **part1.ipynb**: Jupyter notebook containing the implementation and analysis of SARSA and Q-Learning algorithms applied to the gridworld environment. This notebook includes the policy derived from both methods and visualizations of the sum of rewards over episodes.
- **part2.ipynb**: Jupyter notebook covering the implementation of Gradient Monte Carlo and Semi-gradient TD(0) methods. This notebook also compares the value functions obtained from these methods against the exact value function computed using dynamic programming.
- **Images**: The folder contains heatmaps of the value functions computed using different methods:

  - `exact_value_function.png`: Heatmap of the Exact Value Function computed using Dynamic Programming Approach.
  - `gradient_monte_carlo.png`: Heatmap of the Value Function computed using the Gradient Monte Carlo Method.
  - `semi_gradient_td.png`: Heatmap of the Value Function computed using the Semi-Gradient TD(0) Method.

## Methods Overview

### Part 1: SARSA and Q-Learning

- **SARSA**: An on-policy reinforcement learning algorithm that updates the action-value function based on the action taken in the current state and the action taken in the next state.
- **Q-Learning**: An off-policy reinforcement learning algorithm that updates the action-value function by taking the maximum action value for the next state, regardless of the action taken.

### Part 2: Gradient Monte Carlo and Semi-gradient TD(0)

- **Gradient Monte Carlo**: An on-policy method for estimating the value function by updating weights based on the returns observed in each episode.
- **Semi-gradient TD(0)**: An on-policy method that estimates the value function using temporal differences, updating the weights incrementally as the agent interacts with the environment.

### Exact Value Function

- **Dynamic Programming**: Used to compute the exact value function by iteratively updating the value function until convergence. This method is used as a baseline to compare the performance of the reinforcement learning algorithms.

## Getting Started

### Prerequisites

Ensure you have the following installed:

- Python 3.x
- Jupyter Notebook
- Required Python libraries: `numpy`, `matplotlib`, `pandas`

### Running the Notebooks

1. Clone the repository:

   ```bash
   git clone https://github.com/IIsameerII/Reinforcement-Learning-DSCI-6650-003.git
   cd Reinforcement-Learning-DSCI-6650-003
   ```
2. Open the notebooks in Jupyter:

```
jupyter notebook part1.ipynb
jupyter notebook part2.ipynb
```

3. Run the cells in each notebook to execute the code and view the outputs.

## Results

* The notebooks provide detailed outputs including the value functions, policies, and sum of rewards over episodes.
* Heatmaps are generated to visually compare the value functions obtained from different methods.
* The repository demonstrates how different reinforcement learning algorithms perform in a simple gridworld environment.
