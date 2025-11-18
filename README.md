# Trading

Reinforcement Learning Stock Trading (PPO + Custom Gym Environment)
This project demonstrates how a Reinforcement Learning (RL) agent can learn to trade a stock using a custom Gym environment and PPO (Proximal Policy Optimization). The goal is to understand RL concepts and trading logic, not real-world profitability.

# Project Highlights
1. Manual Trading Simulator
A simple interface where the user can:
Buy
Sell
Hold
Auto-advance
It displays price charts, SMA indicators, portfolio value, and trade logs.

3. Custom Gym Trading Environment
The RL environment includes:
State: last 30 prices + cash + position
Actions: Buy (1), Hold (0), Sell (2)
Reward: change in portfolio value
Done: end of dataset

5. PPO Agent Training
A PPO agent is trained on AAPL (2018–2024) data using Stable-Baselines3 and learns trading patterns based on rewards.

# Tech Used
Python, NumPy, Pandas
yfinance
Gym
Stable-Baselines3 (PPO)
Matplotlib
ipywidgets
