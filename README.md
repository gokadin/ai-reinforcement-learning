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
- <img src="/tex/1f1c28e0a1b1708c6889fb006c886784.svg?invert_in_darkmode&sanitize=true" align=middle width=12.67127234999999pt height=14.15524440000002pt/> is the current state of the environment. 
- <img src="/tex/d69e88ed77551b6644e0498dcff34acd.svg?invert_in_darkmode&sanitize=true" align=middle width=34.09118789999999pt height=22.465723500000017pt/> is the immediate reward given the current state <img src="/tex/1f1c28e0a1b1708c6889fb006c886784.svg?invert_in_darkmode&sanitize=true" align=middle width=12.67127234999999pt height=14.15524440000002pt/>. 
- <img src="/tex/ab4745a27f0ed02fe9e696bcff9d032c.svg?invert_in_darkmode&sanitize=true" align=middle width=17.890435199999988pt height=22.465723500000017pt/> is the return, the total reward acquired from time <img src="/tex/90a730292ad140a4739bf15ec17aeed4.svg?invert_in_darkmode&sanitize=true" align=middle width=34.24649744999999pt height=21.18721440000001pt/> to the end of the episode. 
- <img src="/tex/11c596de17c342edeed29f489aa4b274.svg?invert_in_darkmode&sanitize=true" align=middle width=9.423880949999988pt height=14.15524440000002pt/> is the temporal discounting. It makes future rewards less valued than immediate ones. 
- <img src="/tex/9789555e5d8fa5de21171cc40c86d2cd.svg?invert_in_darkmode&sanitize=true" align=middle width=13.65494624999999pt height=14.15524440000002pt/> is an action among a set of possible actions. 
- <img src="/tex/f30fdded685c83b0e7b446aa9c9aa120.svg?invert_in_darkmode&sanitize=true" align=middle width=9.96010619999999pt height=14.15524440000002pt/> is the probability of choosing an action from a set of possible actions given the current state <img src="/tex/1f1c28e0a1b1708c6889fb006c886784.svg?invert_in_darkmode&sanitize=true" align=middle width=12.67127234999999pt height=14.15524440000002pt/> at time <img src="/tex/4f4f4e395762a3af4575de74c019ebb5.svg?invert_in_darkmode&sanitize=true" align=middle width=5.936097749999991pt height=20.221802699999984pt/>. 
- <img src="/tex/aebccd7db45a7ed2bb7db612bc71d08f.svg?invert_in_darkmode&sanitize=true" align=middle width=34.83644339999999pt height=24.65753399999998pt/> is the state value function: the expected long term return based on the current state <img src="/tex/1f1c28e0a1b1708c6889fb006c886784.svg?invert_in_darkmode&sanitize=true" align=middle width=12.67127234999999pt height=14.15524440000002pt/>, or the return <img src="/tex/ab4745a27f0ed02fe9e696bcff9d032c.svg?invert_in_darkmode&sanitize=true" align=middle width=17.890435199999988pt height=22.465723500000017pt/> averaged over all instances of the state <img src="/tex/1f1c28e0a1b1708c6889fb006c886784.svg?invert_in_darkmode&sanitize=true" align=middle width=12.67127234999999pt height=14.15524440000002pt/>. 
- <img src="/tex/f70a068945814ff901edeb2c3d3a8ac1.svg?invert_in_darkmode&sanitize=true" align=middle width=69.97862684999998pt height=24.65753399999998pt/> is the long term return of the current state <img src="/tex/1f1c28e0a1b1708c6889fb006c886784.svg?invert_in_darkmode&sanitize=true" align=middle width=12.67127234999999pt height=14.15524440000002pt/>, taking an action <img src="/tex/9789555e5d8fa5de21171cc40c86d2cd.svg?invert_in_darkmode&sanitize=true" align=middle width=13.65494624999999pt height=14.15524440000002pt/>  under the policy <img src="/tex/f30fdded685c83b0e7b446aa9c9aa120.svg?invert_in_darkmode&sanitize=true" align=middle width=9.96010619999999pt height=14.15524440000002pt/>. 

### Unknown title

The further in time the reward, the less it is valued, as shown by the parameter <img src="/tex/11c596de17c342edeed29f489aa4b274.svg?invert_in_darkmode&sanitize=true" align=middle width=9.423880949999988pt height=14.15524440000002pt/> in the equation below. 

<p align="center"><img src="/tex/f280f6214782a7a38aad847d156ef626.svg?invert_in_darkmode&sanitize=true" align=middle width=437.4738026999999pt height=47.60747145pt/></p>

This equation can also be expressed recursively:

<p align="center"><img src="/tex/cc0cf65ffdd58d46e62d421fecf7f556.svg?invert_in_darkmode&sanitize=true" align=middle width=457.2646056pt height=18.312383099999998pt/></p>

The state value function under a certain policy is the expected long term return of the current state under the given policy. 

<p align="center"><img src="/tex/c7ee076f5276a440b47cb0503aa12b02.svg?invert_in_darkmode&sanitize=true" align=middle width=157.50334875pt height=16.438356pt/></p>

## Code example

🚧UNDER CONSTRUCTION🚧

## References

- Artificial intelligence engines by James V Stone (2019)