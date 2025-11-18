# 📈 RL Stock Trading Demo

This project provides a complete environment for developing and testing Reinforcement Learning (RL) agents for single-asset stock trading. It includes a custom OpenAI Gym environment, an interactive manual trading interface, and a PPO agent trainer using Stable-Baselines3.

---

## ✨ Features

* **Custom Gym Environment (`StockTradingEnv`):** Designed for RL, featuring a continuous action space (buy/sell fraction) and observation space (price window + portfolio state).
* **Interactive Demo (`ManualAgentTrader`):** A Jupyter/Colab interface for manual, step-by-step trading with real-time visualization (price charts, portfolio history).
* **RL Agent Training:** Built-in buttons to **Train** and **Run** a **PPO** (Proximal Policy Optimization) agent directly within the notebook.
* **Real-World Data:** Uses `yfinance` to pull stock data (default: AAPL).
* **Baseline Simulation:** Generates a random trading agent's performance log for comparison.

---

## 🚀 Setup & Installation

This project is best run in a **Google Colab** environment.

### Dependencies

Run the following commands in your notebook environment:

```bash
# Core Dependencies
!pip install --quiet yfinance pandas numpy matplotlib ipywidgets ta

# Reinforcement Learning Dependencies (Required for Agent features)
!pip install stable-baselines3==2.0.0 gym==0.26.2
!pip install torch torchvision torchaudio --index-url [https://download.pytorch.org/whl/cpu](https://download.pytorch.org/whl/cpu)
