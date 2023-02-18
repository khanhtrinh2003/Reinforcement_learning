# Reinforcement_learning
This code is an implementation of the N-Armed Bandit problem and its solution using the epsilon-greedy algorithm. The N-Armed Bandit problem is a classic problem in reinforcement learning where an agent must balance exploration and exploitation of "bandits" (slot machines) to maximize its total reward.

The code consists of two classes:

"Bandit" class: A single bandit with a reward probability defined during instantiation. The class contains methods to get a reward based on the probability and update its mean reward value.

"NArmedBandit" class: This class creates and maintains a list of bandits and implements the epsilon-greedy algorithm to select and update the bandits.

The main methods of the NArmedBandit class are:

- "run": this method selects a bandit using the epsilon-greedy algorithm, gets a reward, and updates the mean reward value.

- "select_bandit": this method implements the epsilon-greedy algorithm to either select a random bandit (with probability epsilon) or the bandit with the maximum mean reward (1-epsilon probability).

- "update": this method updates the mean reward value of the selected bandit.

- "get_bandit_max_q": this method returns the index of the bandit with the maximum mean reward.

- "show_statistics": this method displays the number of times each bandit was selected.
The global constants "EPISODES" and "EPSILON" define the number of iterations and the probability of selecting a random bandit during the run method, respectively. The constant "BANDITS" defines the number of bandits.
