---
title: "Parameter-Efficient Reinforcement Learning via Dynamic Sparse Training"
date: 2024-12-08
description: "Evaluating dynamic sparse training in Advantage Actor-Critic, comparing parameter efficiency and learning stability across classic control and Atari environments."
tags: [reinforcement learning, sparse training, A2C, PPO, research]
---

# Enhancing A2C with DAPD across Classic Control and Atari Environments

*1 Oct 2024 – 10 Dec 2024*

## Project Overview

This project investigates parameter-efficient reinforcement learning through the integration of Dynamic Sparse Training with Pathways (DAPD) into the Advantage Actor-Critic (A2C) algorithm. We compare A2C+DAPD against standard dense A2C and Proximal Policy Optimization (PPO) across three benchmark environments—LunarLander-v2, Breakout, and Pong—to evaluate trade-offs between computational efficiency and learning reliability.

## Full Report

Access the full details about the project and result on the [Project Report](final_report.pdf).

## Presentation

<iframe 
    src="https://1drv.ms/v/c/891814256f52dec4/IQR9BlTeSsQdQ7ZWnndV-xzfATA8fk1T9Z-vk3O7rcD_LRk" 
    width="1440" 
    height="1080" 
    frameborder="0" 
    scrolling="no" 
    allowfullscreen>
</iframe>

## Objectives

- Assess the impact of DAPD on A2C’s training speed and parameter footprint.
- Compare performance and stability of sparse and dense agents across classic and visual control tasks.
- Derive empirical insights into the trade-offs inherent in dynamic sparse training within RL.

## Technical Approach

- **A2C**: Advantage Actor-Critic with actor and critic networks sharing a two-layer feed-forward architecture (64 ReLU units), optimized via Adam.
- **PPO**: Dense baseline using a clipped objective for enhanced stability and sample efficiency.
- **A2C+DAPD**: Incorporates a binary mask to maintain 90% sparsity, updating prune–regrow operations periodically (every 1,000 steps for LunarLander; 100,000 for Atari).

Agents are trained for 10,000 episodes in each environment, recording episodic rewards, average performance over the last 100 episodes, and wall-clock training time. Reward curves are smoothed using a 100-episode moving average.

## Experiments

We evaluate:

- **LunarLander-v2**: Classic control task, low-dimensional state space.
- **Breakout & Pong**: Visual environments from the Atari suite.

Key findings:
- DAPD reduces wall-clock training time by approximately 30–40%, converging in ~8,000–14,000 seconds versus ~14,000–25,000 seconds for dense A2C.
- Sparse training introduces significant variance and instability, particularly in control tasks.
- PPO consistently outperforms both A2C variants in final reward and stability across all environments.

## Outcomes and Future Work

Our results highlight the computational advantages of dynamic sparse training at the expense of convergence reliability. While DAPD accelerates early learning, its instability underscores the need for sparsity-aware optimization strategies. Future directions include:

- Thorough evaluation of the Policy Pruning and Shrinking (PoPS) method.
- Exploration of structured sparsity, adaptive pruning schedules, and hybrid dense–sparse models.
- Deployment studies on resource-constrained hardware for real-time applications.
