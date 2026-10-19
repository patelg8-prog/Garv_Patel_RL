## Author
**Garv Patel**  
Module: Generative AI and Reinforcement Learning  
Task 2: Reinforcement Learning

## Overview
Reinforcement learning for the Chef’s Hat card game using the **Chef’s Hat Gym environment**.

The project compares:
- **Baseline:** Dueling Deep Q-Network (DQN)
- **Reward Shaping:** DQN with potential-based reward shaping

## Environment
**Chef’s Hat Gym**

- Environment: Multi-agent card game
- State representation: 28-dimensional
- Action handling: Action masking
- Variant: Sparse / Delayed Reward
- Objective: Investigate the effect of reward shaping on agent performance

## Algorithm
**Dueling Deep Q-Network (DQN)**

The baseline agent learns from the environment's reward signal, while the reward-shaped agent uses an additional potential-based shaping reward.

## Evaluation
Metrics:
- Win rate
- Average finishing position
- Average reward
- Training loss and exploration rate

Final results:

| Model | Win Rate | Avg. Position | Avg. Reward |
|---|---:|---:|---:|
| Baseline DQN | 25% | 2.50 | 0.735 |
| Reward-Shaped DQN | 25% | 2.50 | 0.735 |

## Main Finding
The reward-shaped agent showed no overall improvement over the baseline in the reported experiment. Further training and evaluation are needed to investigate the effectiveness of reward shaping.

## Limitations
- Limited evaluation runs.
- Reward-shaping parameters may require further optimisation.
