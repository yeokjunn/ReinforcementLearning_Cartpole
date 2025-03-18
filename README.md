# Reinforcement Learning for CartPole

## Overview
This project implements two different reinforcement learning approaches to solve the classic CartPole balancing problem from OpenAI Gym/Gymnasium:
1. Q-Learning with state discretization
2. Policy Gradient with a baseline value function

The CartPole problem involves balancing a pole attached to a moving cart by applying appropriate forces to keep the pole upright.

## Project Structure
- `SC3000_ProjectCartpole_KeJun.ipynb`: Main Jupyter notebook containing all implementations and explanations
- `q_learning_cartpole_model.pkl`: Saved Q-Learning model
- `q_learning_cartpole_complete.pkl`: Saved Q-Learning parameters and hyperparameters
- `video/`: Directory containing rendered videos of trained agents

## Implementations

### Q-Learning Agent
- Uses state discretization to handle the continuous state space
- Implements epsilon-greedy exploration strategy
- Features automatic epsilon decay for better exploitation over time
- Achieves "solved" status (average reward > 195 over 100 episodes)

### Policy Gradient Agent
- Neural network-based approach using TensorFlow
- Implements a baseline value function to reduce variance
- Uses entropy regularization for better exploration
- Gradient clipping for training stability

## Key Features
- Comprehensive implementation of both tabular and neural network RL approaches
- Detailed explanations of mathematical foundations
- Performance visualization and comparison
- Video rendering of trained agents in action

## Requirements
- Python 3.x
- TensorFlow
- NumPy
- Matplotlib
- OpenAI Gym/Gymnasium
- Pickle

## Usage
1. Open the Jupyter notebook `SC3000_ProjectCartpole_KeJun.ipynb`
2. Run the cells in order to train and evaluate both agents
3. View the rendered videos to see the agents in action

## Results
Both agents successfully learn to balance the pole, with the Q-Learning agent achieving an average reward of over 195 across 100 episodes, meeting the "solved" criterion for the CartPole environment.

