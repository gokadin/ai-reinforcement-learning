# Reinforcement learning

Reinforcement learning explained and demonstrated. 

## This is part X of a series of github repos on neural networks

- [part 1 - simplest network](https://github.com/gokadin/ai-simplest-network)
- [part 2 - backpropagation](https://github.com/gokadin/ai-backpropagation)
- [part 3 - backpropagation-continued](https://github.com/gokadin/ai-backpropagation-continued)

## Table of Contents

- [Theory](#theory)
  - [Notation](#notation)
- [Code example](#code-example)
- [References](#references)

## Theory

🚧UNDER CONSTRUCTION🚧

### Notation

- An *episode* is the total sequence of states for a given scenario, for example a game. 
- An *agent* is the entity being trained that performs actions in an environment and gains rewards. 
- $s_t$ is the current state of the environment. 
- $R_{t + 1}$ is the immediate reward given the current state $s_t$. 
- $G_t$ is the return, the total reward acquired from time $t + 1$ to the end of the episode. 
- $\gamma$ is the temporal discounting. It makes future rewards less valued than immediate ones. 
- $a_t$ is an action among a set of possible actions. 
- $\pi$ is the probability of choosing an action from a set of possible actions given the current state $s_t$ at time $t$. 
- $v(s_t)$ is the state value function: the expected long term return based on the current state $s_t$, or the return $G_t$ averaged over all instances of the state $s_t$. 
- $Q_\pi(s_t, a_t)$ is the long term return of the current state $s_t$, taking an action $a_t$  under the policy $\pi$. 

### Unknown title

The further in time the reward, the less it is valued, as shown by the parameter $\gamma$ in the equation below. 

$$ G_t = R_{t+1} + \gamma R_{t+2} + \gamma^2 R_{t+3} + \gamma^3 R_{t+4} + ... = \sum^N_{n=0} \gamma^n R_{t+n+1} $$

This equation can also be expressed recursively:

$$ G_t = R_{t+1} + \gamma(R_{t+2} + \gamma R_{t+3} + \gamma^2 R_{t+4} + ...) = R_{t+1} + \gamma(G_{t+1}) $$

The state value function under a certain policy is the expected long term return of the current state under the given policy. 

$$ V_\pi(s) = E_\pi[G_t|s_t = s] $$

## Code example

🚧UNDER CONSTRUCTION🚧

## References

- Artificial intelligence engines by James V Stone (2019)