---
title: 'Capture-recapture models for Halo: Infinite online'
date: 2022-12-18
permalink: /posts/2022/12/halo-crc/
tags:
  - fun projects
---

Capture-recapture models (CRC), or Multiple Systems Estimation models, operate on an initially simple premise: if you take multiple samples, a small population means that individuals are more likely to appear in multiple samples. These 'samples' can appear in many applications, though they originated in ecological experiments to estimate the abundance of a certain animal in certain areas. An initial sample of animals is taken, each animal in that sample is marked and released, and at some later time, another sample is taken. The number of marked animals that appear in that second sample can give an estimate of the total population size. In other applications, these methods have been used to estimate the total population size in hard-to-track populations, such as homeless people or [victims of human rights violations.](https://hrdag.org/2013/03/11/mse-the-basics/) 

This little project arose because my partner plays online matches of Halo: Infinite (a science fiction first-person shooter) almost every night after work. After enough games, she started to see the same players appear multiple times. I decided to collect some data and practice some CRC modeling with it to estimate the total number of players who are using Halo: Infinite online.

For each match, a player is paired with 15 others to form two teams of 8 people. Each player has a persistent player username, so they can be tracked between matches. Though I do not know the exact details of how players are paired, I treat each match as a "sample" of 15 other players then.

Over the course of 16 matches (and I continue to collect data!), I logged the date of the sample and the usernames of the players in each game.

Here's a sample of what the data looked like:


A Simple Bayesian Capture-Recapture model
-----
