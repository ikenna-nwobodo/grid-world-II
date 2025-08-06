# Gridworld

This project implements two classic reinforcement learning algorithms — **SARSA** and **Q-Learning** — to solve a 5x5 gridworld navigation problem with special states and terminal rewards. The goal is to learn optimal policies through interaction with the environment and visualize the learned trajectories.

## Project Structure

- `sarsa()`: Implements the SARSA algorithm with an epsilon-greedy policy.
- `qlearn()`: Implements the Q-Learning algorithm using off-policy updates.
- `plot_trajectory(Q, title)`: Visualizes the trajectory taken by an agent following the learned policy.
- `select_action()`: Chooses actions using an epsilon-greedy strategy.
- `ns_reward()`: Simulates state transitions, rewards, and termination logic.
- `state_idx`: Maps grid coordinates to Q-table indices.

## Algorithms

### SARSA
An on-policy algorithm that updates Q-values based on the action actually taken in the next step.

### Q-Learning
An off-policy algorithm that updates Q-values based on the maximum possible future Q-value, regardless of the next action actually taken.

## Environment Overview

- **Grid size**: 5x5
- **Special states**:
  - `Blue`: Starting state
  - `Red`: Obstacle
  - `Black`: Terminal states
- **Rewards**:
  - -20 for hitting obstacle
  - -1 for regular moves
  - -1 for moving off grid

## How to Run

1. Clone this repository
2. Ensure you have `matplotlib` and `numpy` installed
