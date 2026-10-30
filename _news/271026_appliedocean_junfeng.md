---
layout: post
title: 🎉 Paper published to Applied Ocean Research by Junfeng Xue
date: 2026-10-27 00:00:00-0400
inline: false
related_posts: false
tags: publishing
---

Junfeng Xue, together with Yuanchang Liu, has published a new paper, [A biomimetic learning acceleration strategy on reinforcement learning for obstacle-aware end-to-end path planning of USV](https://www.sciencedirect.com/science/article/pii/S0141118726003779), addressing a key challenge in autonomous surface vehicle (USV) navigation: improving the training efficiency of reinforcement learning models for end-to-end path planning and obstacle avoidance in complex marine environments.

The work introduces a biomimetic learning acceleration (BLA) strategy designed to accelerate reinforcement learning during the initial stages of training. The proposed approach consists of three complementary modules: learning-process segmentation, reward reinforcement, and exploration-efficiency enhancement. Together, these modules guide the learning process towards more promising regions, strengthen reward propagation between successful and failed actions, and reduce redundant exploration of potentially unsafe actions.

A central contribution of the study is the integration of prior feasible regions, sub-risk regions, and recorded successful trajectories into the reinforcement learning process. By identifying potentially dangerous actions and preserving promising exploration paths, the strategy improves learning efficiency while helping the agent develop effective obstacle-aware navigation behaviours.

The proposed method is evaluated through simulation using an Implicit Quantile Network (IQN). The results demonstrate a substantial improvement in early-stage learning performance, increasing the success rate from 60.0% to 93.3% with just 120 seconds of training. These findings highlight the potential of biomimetic learning strategies to accelerate reinforcement learning for autonomous marine navigation.