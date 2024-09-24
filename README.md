# Deep Q-Learning for Lunar Lander 🚀

This project implements a **Deep Q-Learning** agent to solve the classic **Lunar Lander** environment from OpenAI Gym. The agent is trained to land a lunar module safely using reinforcement learning techniques. The project features customizable hyperparameters, experience replay, and epsilon-greedy exploration strategies.

## 📋 Project Overview

The Lunar Lander environment involves guiding a spacecraft to land on the surface of the moon safely. The agent is rewarded for smooth landings and penalized for crashing or flying out of bounds. The challenge is to train a neural network to choose the best actions based on the state of the lander.

This project uses **Deep Q-Learning (DQN)**, a reinforcement learning algorithm where the agent learns a policy by estimating Q-values for state-action pairs and optimizing its behavior through trial and error.

## 🧠 Key Features

- **Deep Q-Network (DQN):** Neural network architecture with experience replay.
- **Replay Memory:** Stores agent experiences to improve learning stability.
- **Epsilon-Greedy Exploration:** Balances exploration of new actions and exploitation of known rewards.
- **Customizable Hyperparameters:** Allows fine-tuning of learning rates, buffer size, and other key factors.
- **Gym Environment:** The project is based on OpenAI's Lunar Lander-v2 environment.

## 🛠️ Requirements

To run the project, you'll need the following dependencies:

```bash
pip install gymnasium[box2d] torch numpy
```

## 🚀 Getting Started

### Clone the Repository:

```bash
git clone https://github.com/sudhersankv/Deep_Q_Learning_Lunar_Lander.git
cd Deep_Q_Learning_Lunar_Lander
```

### Run the Notebook:

Use Jupyter or a similar notebook environment to run the provided `.ipynb` file.

```bash
jupyter notebook Deep_Q_Learning_for_Lunar_Landing.ipynb
```

### Customizing Parameters

You can adjust the hyperparameters like learning rate, discount factor, replay buffer size, and epsilon decay inside the notebook.

```python
learning_rate = 5e-4
gamma = 0.99
epsilon_start = 1.0
epsilon_end = 0.01
epsilon_decay_rate = 0.995
```

## 🎮 Running the Agent

Once the environment is set up, and you run the notebook, the agent will train on the Lunar Lander environment. Here's an overview of the training process:

### Training Process

- **Replay Buffer Size**: `1e5` 
- **Epsilon Decay**: `0.995`
- **Batch Size**: `100`
- **Learning Rate**: `5e-4`

### Training Results

During training, the agent's performance improves over time. Below is a summary of the average score achieved per episode over 1,000 episodes:

	Episode 100: Average Score: -187.99
	Episode 200: Average Score: -113.49
	Episode 300: Average Score: -50.73
	Episode 400: Average Score: 27.15
	Episode 500: Average Score: 130.50
	Episode 600: Average Score: 178.59
	Episode 700: Average Score: 200.64

Environment solved in 600 episodes! The final trained agent achieves a consistent average score of 200.64.

**Final Score:** `200.64`

The final trained agent is capable of successfully landing the Lunar Lander module consistently, earning a stable score around 200.

## 📚 References

- [OpenAI Gym](https://gym.openai.com/)
- [Deep Q-Learning Paper](https://arxiv.org/abs/1312.5602)

## 🧑‍💻 Author

This project was developed by **Sudhersan K V**. Feel free to reach out for questions or suggestions.

## 🤝 Contributions

Contributions are welcome! Feel free to fork this project, submit issues, or open pull requests.

## 📜 License

This project is licensed under the MIT License.

