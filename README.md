# Hopfield networks

Hopfield networks explained and demonstrated. 

## This is part 4 of a series of github repos on neural networks

- [part 1 - simplest network](https://github.com/gokadin/ai-simplest-network)
- [part 2 - backpropagation](https://github.com/gokadin/ai-backpropagation)
- [part 3 - backpropagation-continued](https://github.com/gokadin/ai-backpropagation-continued)
- part 4 - hopfield-networks (**you are here**)

## Table of Contents-

- [Theory](#theory)
  - [A different type of network](#a-different-type-of-network)
  - [Learning](#learning)
- [Code example](#code-example)
- [References](#references)

## Theory

### A different type of network

Hopfield networks are are a type of artificial neural networks that have fully interconnected nodes as opposed to layers. In the case of the image below, there are 7 nodes each connected to 6 other nodes with outgoing and incoming weight values. This mearns that each node is both an input and an output of the network. 

Hopfield networks and Boltzmann machines are known as energy based networks, meaning they are associating a scalar energy to each configuration of variables. 

Its main use is to learn an association between an input and output and recall the learned pattern based on a corrupted, partial or noisy input. 

![hopfield-network](readme-images/hopfield-net.jpg)

If <img src="/tex/d6328eaebbcd5c358f426dbea4bdbf70.svg?invert_in_darkmode&sanitize=true" align=middle width=15.13700594999999pt height=22.465723500000017pt/> is the total number of nodes, then the input to each node <img src="/tex/4d8443b72a1de913b4a3995119296c90.svg?invert_in_darkmode&sanitize=true" align=middle width=15.499497749999989pt height=14.15524440000002pt/> is the sum of other node outputs <img src="/tex/2b442e3e088d1b744730822d18e7aa21.svg?invert_in_darkmode&sanitize=true" align=middle width=12.710331149999991pt height=14.15524440000002pt/> times their corresponding weights <img src="/tex/64e70e84545b2941bed8aa7fe2211cde.svg?invert_in_darkmode&sanitize=true" align=middle width=22.523917349999987pt height=14.15524440000002pt/> minus the bias unit <img src="/tex/2020a79c00e140ee1a054ecab57a289c.svg?invert_in_darkmode&sanitize=true" align=middle width=13.15930604999999pt height=22.831056599999986pt/>. 

<p align="center"><img src="/tex/7e8492417836f21c62678780206ed8aa.svg?invert_in_darkmode&sanitize=true" align=middle width=136.30514205pt height=47.806078649999996pt/></p>

As we did in *part 2 and 3*, if we count the bias node as a regular input to a node, then we can simplify the equation:

<p align="center"><img src="/tex/d1417a3cc7502763de5bb13b80305ca5.svg?invert_in_darkmode&sanitize=true" align=middle width=106.983987pt height=47.806078649999996pt/></p>

Hopfield network node outputs are binary (we'll use <img src="/tex/c11fe0cea175e1b787b3403c763dc9b0.svg?invert_in_darkmode&sanitize=true" align=middle width=21.00464354999999pt height=21.18721440000001pt/> and <img src="/tex/e11a8cfcf953c683196d7a48677b2277.svg?invert_in_darkmode&sanitize=true" align=middle width=21.00464354999999pt height=21.18721440000001pt/>) and make use of an activation function <img src="/tex/190083ef7a1625fbc75f243cffb9c96d.svg?invert_in_darkmode&sanitize=true" align=middle width=9.81741584999999pt height=22.831056599999986pt/> that transforms their input to either <img src="/tex/c11fe0cea175e1b787b3403c763dc9b0.svg?invert_in_darkmode&sanitize=true" align=middle width=21.00464354999999pt height=21.18721440000001pt/> if <img src="/tex/4d7eade3107e105984e8ad3fa0f5aa41.svg?invert_in_darkmode&sanitize=true" align=middle width=46.45823159999998pt height=21.18721440000001pt/> and <img src="/tex/e11a8cfcf953c683196d7a48677b2277.svg?invert_in_darkmode&sanitize=true" align=middle width=21.00464354999999pt height=21.18721440000001pt/> if <img src="/tex/d37fa122c68a9c2c80ae2bff336e140d.svg?invert_in_darkmode&sanitize=true" align=middle width=46.45823159999998pt height=21.18721440000001pt/>. 

### Learning

🚧UNDER CONSTRUCTION🚧

## Code example

🚧UNDER CONSTRUCTION🚧

## References

- Artificial intelligence engines by James V Stone (2019)