# Project : CartPole Balance Agent using Reinforcement Learning

## 1) Project Overview

This project trains an agent to balance a pole on a moving cart by choosing left or right actions. The agent learns from reward feedback through interaction with the environment. It is a reinforcement learning project and uses a perceptron-style policy network.

## 2) Dataset Summary

* **Dataset / Environment Name:** CartPole-v1
* **Source:** Gymnasium
* **Type:** Reinforcement learning environment
* **State Space:** 4 values

  * cart position
  * cart velocity
  * pole angle
  * pole angular velocity
* **Action Space:** 2 actions

  * move left
  * move right
* **Reward:** +1 for every time step the pole stays balanced

## 3) Workflow

1. Create the CartPole environment
2. Observe the current state
3. Pass the state into the perceptron policy network
4. Convert model output into action probabilities using Softmax
5. Sample an action from the probability distribution
6. Apply the action in the environment
7. Receive the next state and reward
8. Store transitions such as state, action, reward, and next state
9. Compute discounted returns
10. Update policy weights using policy gradient learning
11. Repeat over many episodes until performance improves

## 4) Key Result

The trained agent learns to keep the pole balanced for longer episodes, which means the average reward increases during training.

## 5) Machine Learning Model

* **Model Type:** Perceptron-style policy network
* **Network Structure:** Single linear layer
* **Action Selection:** Softmax + Categorical sampling
* **Learning Method:** Policy Gradient style update

## 6) Association Rule

Association rule mining is not applicable to this project because reinforcement learning is based on sequential decision-making and reward feedback, not pattern discovery from item co-occurrence.

## 7) Unique Thing About the Project

* Uses a classic RL benchmark environment
* Very standard and easy to explain in viva
* Perceptron-style policy keeps the project simple and lightweight
* Can also save transitions as a CSV dataset for presentation

## 8) Viva Explanation Points

* This is a reinforcement learning project
* There is no fixed labeled dataset
* The agent learns from rewards received after actions
* The policy network maps state to action probabilities
* Softmax is used to convert raw scores into probabilities
* Discounted returns help value future rewards
* The project shows how an agent improves by trial and error

## 9) Good Viva Questions

1. What is reinforcement learning?
2. What is the state in CartPole?
3. What are the actions available to the agent?
4. Why is this not supervised learning?
5. Why is Softmax used?
6. What does the reward mean?
7. What is the role of the perceptron here?
8. Why do we compute discounted returns?
9. How does the policy improve over time?
10. What is the difference between exploration and exploitation?

## Project Code Link

[https://colab.research.google.com/drive/1T6tPZMXHRE3TVPeoHtZeB6AR19EePJeQ?usp=sharing](https://colab.research.google.com/drive/1T6tPZMXHRE3TVPeoHtZeB6AR19EePJeQ?usp=sharing)

## Technologies Used

* Python
* PyTorch
* Gymnasium
* NumPy
* Matplotlib
* Google Colab

## Final Note

This project demonstrates reinforcement learning through a simple but powerful control task, making it an excellent choice for college viva and practical understanding.
