<!--- Banner -->
<br />
<p align="center">
<a href="#"><img src="https://i.ibb.co/CnqrM5t/image.png"></a>
<h3 align="center">Multi-Armed Bernoulli Bandits</h3>
<p align="center">An exploration of multi-armed Bernoulli bandits in reinforcement learning, complete with experiments and observations.</p>

<!--- About --><br />
## About
The notebook is an exploration of multi-armed Bernoulli bandits in reinforcement learning. These bandits are a simplified but essential concept in Reinforcement Learning, where an agent must decide between multiple arms to pull, each with an unknown probability of giving a reward. Bernoulli bandits provide rewards with a binary outcome, typically 0 or 1. The objective is to devise a strategy that maximizes the expected sum of rewards over a sequence of pulls.

<!--- Experiments --><br />
## Experiments

The first strategy employed was the ϵ-greedy approach. In this strategy, the agent either exploits the arm with the highest known reward with probability 1−ϵ or explores a random arm with probability ϵ. Experiments were conducted to analyze the impact of this approach in both stationary and non-stationary settings, and to observe the effects of changes in the underlying reward distribution.

To improve upon the ϵ-greedy strategy, a decaying ϵ was introduced. This approach allowed the agent to focus more on exploiting known information as it gained experience. Experiments were performed in non-stationary Bernoulli bandit settings where reward probabilities change over time.

The final set of experiments introduced Boltzmann exploration as an alternative to ϵ-greedy. In Boltzmann exploration, arms are selected based on a probabilistic distribution that is influenced by the estimated value of those arms. This strategy was also put through various test scenarios, and its performance was evaluated.
