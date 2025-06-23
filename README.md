# EcoTradeAI-ESG-Aware-Reinforcement-Learning-for-Real-Time-Compute-Resource-Optimization

# 🌍 EcoTradeAI

> ESG-Aware Reinforcement Learning Agent for Real-Time Compute Resource Optimization  
> **Built for MARA Hackathon 2025** · Simulated API Environment

---

## 🧠 What is EcoTradeAI?

**EcoTradeAI** is an intelligent agent that dynamically allocates compute resources (ASICs, GPUs, mining rigs) across a simulated energy-inference marketplace, aiming to **maximize profit** while **minimizing ESG costs** like carbon emissions, water consumption, and e-waste.

The project was built in real-time during the [MARA Hackathon 2025] using a **simulated marketplace API provided by MARA**. All price and market data used are synthetic and not representative of real-world values.

---

## 🚀 Key Features

- ♻️ **EcoReward Optimization**: Balances profit with environmental penalties using custom α, β, γ, δ weights
- 📉 **Real-Time Streamlit Dashboard**: Visualizes live metrics on price, power usage, CO₂ emissions, and revenue
- 📦 **RL Agent using PPO**: Trained using Stable Baselines3 on a custom OpenAI Gym-style environment
- 🔁 **Live API Integration**: Agent allocates resources via MARA’s simulated `PUT /machines` endpoint
- 📊 **Dynamic Strategy Comparison**: Benchmark performance against random and rule-based policies

---

## 📸 UI Preview

<img width="1427" alt="image" src="https://github.com/user-attachments/assets/1eb211c9-2dfd-4a57-ac82-c1959d35c78b" />

---

## 🗂️ Project Structure

```bash
.
├── streamlit_app.py          # Main dashboard
├── agent.py                  # RL agent loop
├── train_ppo.py              # PPO training script
├── utils/
│   ├── charts.py             # Custom Streamlit charts
│   ├── mara_env.py           # Custom Gym environment
├── ppo_mara_agent.zip        # Pretrained PPO model
├── data/
│   └── metrics.csv           # Logged metrics
├── requirements.txt          # Python dependencies
└── README.md
