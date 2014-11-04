---
layout: post
title: FIFA World Cup Prediction Project
author: Anant Agarwal
excerpt: Notes on the current state of the project and possible extensions.
---


## FIFA World Cup Prediction System

Here are a few details of the talk I had given today regarding the prediction system -

Description -

	+ The system is a very naive implementation that uses only past world cup information from 1950 - 2014
	+ The system uses a single hidden node neural network using PyBrain
	+ The system does some minor EDA to see the distribution of team's performance.
	+ The features used are win%, loss%, podiumFinish%, goalDiff etc.

Extensions -

	+ Add player specific features such that presence of a strong player (in form) has an effect on the result.
	+ Add "non-world" specific information
	+ Consider the performance of a team over the years.


The github link is - https://github.com/anantag/FIFAWorldCup2014_NeuralNetworkPrediciton 

I will make sure to update the readme with more detailed info and step to run the program, dependencies etc.

Meanwhile, please feel free to look at the link and make further suggestions.

Thanks,
Anant.
