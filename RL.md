Reinforcement Learning: An Introduction
=======

Author: Richard S. Sutton and Andrew G. Barto

PDF: [Reinforcement Learning 2016sep.pdf](http://incompleteideas.net/sutton/book/bookdraft2016sep.pdf)

Website: http://incompleteideas.net/sutton/index.html

Contents
------
![](../master/RL_png/image001.png?raw=true)
![](../master/RL_png/image002.png?raw=true)
![](../master/RL_png/image003.png?raw=true)
![](../master/RL_png/image004.png?raw=true)
![](../master/RL_png/image005.png?raw=true)
![](../master/RL_png/image006.png?raw=true)

Notation
------
![](../master/RL_png/image007.png?raw=true)
![](../master/RL_png/image008.png?raw=true)

1.3 Elements of Reinforcement Learning
------
   a policy, a reward signal, a value function, a model of the environment.

Part I: Tabular Solution Methods
======

2 Multi-arm Bandits
======
greedy:

![](../master/RL_png/image010.png?raw=true)

![](../master/RL_png/image011.png?raw=true)

ε-greedy:

![](../master/RL_png/image012.png?raw=true)

Tracking a Nonstationary Problem

![](../master/RL_png/image013.png?raw=true)

![](../master/RL_png/image014.png?raw=true)

Optimistic Initial Values

![](../master/RL_png/image015.png?raw=true)

UCB(upper conidence bound): // UCT: UCB for Tree

![](../master/RL_png/image016.png?raw=true)

![](../master/RL_png/image017.png?raw=true)

GBA(Gradient Bandit Algorithms):

![](../master/RL_png/image018.png?raw=true)

![](../master/RL_png/image019.png?raw=true)

![](../master/RL_png/image020.png?raw=true)

![](../master/RL_png/image021.png?raw=true)
![](../master/RL_png/image022.png?raw=true)
![](../master/RL_png/image023.png?raw=true)

2.9 Summary
------

![](../master/RL_png/image024.png?raw=true)

3 Finite Markov Decision Processes
======
![](../master/RL_png/image025.png?raw=true)

episodic:

![](../master/RL_png/image026.png?raw=true)

continuing tasks:

![](../master/RL_png/image027.png?raw=true), ![](../master/RL_png/image028.png?raw=true)

continuing tasks or episodic:

![](../master/RL_png/image029.png?raw=true)

![](../master/RL_png/image030.png?raw=true)

3.5 The Markov Property
------
![](../master/RL_png/image031.png?raw=true)

3.6 Markov Decision Processes
------
the probability of each possible pair of next state and reward

![](../master/RL_png/image032.png?raw=true)

expected rewards for state,action pairs

![](../master/RL_png/image033.png?raw=true)

state-transition probabilities

![](../master/RL_png/image034.png?raw=true)

3.7 Value Function
------
![](../master/RL_png/image035.png?raw=true)

![](../master/RL_png/image036.png?raw=true)

![](../master/RL_png/image037.png?raw=true)

![](../master/RL_png/image038.png?raw=true)

the value of a state s under a policy π

![](../master/RL_png/image039.png?raw=true)

the value of taking action a in state s under a policy π

![](../master/RL_png/image040.png?raw=true)

Bellman equation for Vπ

![](../master/RL_png/image041.png?raw=true)

3.8 Optimal Value Functions
------
optimal state-value function

![](../master/RL_png/image042.png?raw=true)

optimal action-value function

![](../master/RL_png/image043.png?raw=true)

![](../master/RL_png/image044.png?raw=true)

Bellman optimality equation for v*

![](../master/RL_png/image045.png?raw=true)

Bellman optimality equation for q*

![](../master/RL_png/image046.png?raw=true)

4 Dynamic Programming
======

![](../master/RL_png/image047.png?raw=true)

![](../master/RL_png/image048.png?raw=true)

4.1 Policy Evaluation
------
![](../master/RL_png/image049.png?raw=true)

![](../master/RL_png/image050.png?raw=true)

![](../master/RL_png/image051.png?raw=true)

4.2 Policy Improvement
------
![](../master/RL_png/image052.png?raw=true)

![](../master/RL_png/image053.png?raw=true)

Prove:

![](../master/RL_png/image054.png?raw=true)

4.3 Policy Iteration
------
Process:

![](../master/RL_png/image055.png?raw=true)

Formula:

![](../master/RL_png/image056.png?raw=true)

![](../master/RL_png/image057.png?raw=true)

Algorithm:

![](../master/RL_png/image058.png?raw=true)

4.4 Value Iteration
------
Formula:

![](../master/RL_png/image059.png?raw=true)

Algorithm:

![](../master/RL_png/image060.png?raw=true)

Additional: Modified Policy Iteration

* P203: Markov Decision Processes Discrete Stochastic Dynamic Programming
* P21: CS294 RL definitions, value iteration, policy iteration -> slide


4.6 Generalized Policy Iteration
------
![](../master/RL_png/image061.png?raw=true)
![](../master/RL_png/image062.png?raw=true)

5 Monte Carlo Methods
======

![](../master/RL_png/image063.png?raw=true)

![](../master/RL_png/image064.png?raw=true)

First-visit MC, every-visit MC

![](../master/RL_png/image065.png?raw=true)

5.2 Monte Carlo Estimation of Action Values
------

5.3 Monte Carlo Control
------
![](../master/RL_png/image066.png?raw=true)

![](../master/RL_png/image067.png?raw=true)

![](../master/RL_png/image068.png?raw=true)

![](../master/RL_png/image069.png?raw=true)

![](../master/RL_png/image070.png?raw=true)

![](../master/RL_png/image071.png?raw=true)

5.4 Monte Carlo Control without Exploring Starts
------
![](../master/RL_png/image072.png?raw=true)

![](../master/RL_png/image073.png?raw=true)

5.5 Off-policy Prediction via Importance Sampling
------
[Importance Sampling](https://en.wikipedia.org/wiki/Importance_sampling)

5.6 Incremental Implementation
------
![](../master/RL_png/image074.png?raw=true)

5.7 Off-Policy Monte Carlo Control
------
![](../master/RL_png/image075.png?raw=true)

6 Temporal-Difference Learning
======

![](../master/RL_png/image076.png?raw=true)

![](../master/RL_png/image077.png?raw=true)

TD-error:

![](../master/RL_png/image078.png?raw=true)

MC-error:

![](../master/RL_png/image079.png?raw=true)

6.2 Advantages of TD Prediction Methods
------
![](../master/RL_png/image080.png?raw=true)

![](../master/RL_png/image081.png?raw=true)

6.4 Sarsa: On-Policy TD Control
------
![](../master/RL_png/image082.png?raw=true)

6.5 Q-learning: Off-Policy TD Control
------
![](../master/RL_png/image083.png?raw=true)

6.6 Expected Sarsa
------
![](../master/RL_png/image084.png?raw=true)

![](../master/RL_png/image085.png?raw=true)

6.7 Maximization Bias and Double Learning
------
![](../master/RL_png/image086.png?raw=true)

![](../master/RL_png/image087.png?raw=true)

![](../master/RL_png/image088.png?raw=true)

6.8 Games, Afterstates, and Other Special Cases
------
![](../master/RL_png/image089.png?raw=true)

7 Multi-step Bootstrapping
======

7.1 n-step TD Prediction
------
![](../master/RL_png/image090.png?raw=true)

![](../master/RL_png/image091.png?raw=true)

![](../master/RL_png/image092.png?raw=true)

![](../master/RL_png/image093.png?raw=true)

7.2 n-step Sarsa
------
![](../master/RL_png/image094.png?raw=true)

![](../master/RL_png/image095.png?raw=true)

7.3 n-step Off-policy Learning by Importance Sampling
------
![](../master/RL_png/image096.png?raw=true)

![](../master/RL_png/image097.png?raw=true)

![](../master/RL_png/image098.png?raw=true)

![](../master/RL_png/image099.png?raw=true)

![](../master/RL_png/image100.png?raw=true)

7.4 Off-policy Learning Without Importance Sampling: The n-step Tree Backup Algorithm
------
![](../master/RL_png/image101.png?raw=true)

![](../master/RL_png/image102.png?raw=true)

![](../master/RL_png/image103.png?raw=true)

7.5 A Unifying Algorithm: n-step Q(σ)
------
![](../master/RL_png/image104.png?raw=true)
![](../master/RL_png/image105.png?raw=true)

![](../master/RL_png/image106.png?raw=true)

8 Planning and Learning with Tabular Methods
======

![](../master/RL_png/image107.png?raw=true)

![](../master/RL_png/image108.png?raw=true)

![](../master/RL_png/image109.png?raw=true)

8.1 Models and Planning
------
![](../master/RL_png/image110.png?raw=true)

![](../master/RL_png/image111.png?raw=true)

8.2 Dyna: Integrating Planning, Acting, and Learning
------
![](../master/RL_png/image112.png?raw=true)

![](../master/RL_png/image113.png?raw=true)

![](../master/RL_png/image114.png?raw=true)

![](../master/RL_png/image115.png?raw=true)

8.3 When the Model Is Wrong
------
![](../master/RL_png/image116.png?raw=true)

![](../master/RL_png/image117.png?raw=true)

8.4 Prioritized Sweeping
------
![](../master/RL_png/image118.png?raw=true)

![](../master/RL_png/image119.png?raw=true)

8.6 Heuristic Search
------
Alpha-Beta, MCTS ...

8.7 Monte Carlo Tree Search
------
Reference:

* 2006 Modiﬁcation of UCT with Patterns in Monte-Carlo Go.pdf
* 2009 Reinforcement Learning and Simulation-Based Search in Computer Go.pdf
* 2011 New Heuristics for Monte Carlo Tree Search Applied to the Game of Go.pdf

Part II: Approximate Solution Methods
======

9 On-policy Prediction with Approximation
======
![](../master/RL_png/image120.png?raw=true)

9.2 The Prediction Objective (MSVE)
------
Mean Squared Value Error, or MSVE:

![](../master/RL_png/image121.png?raw=true)

![](../master/RL_png/image122.png?raw=true)

9.3 Stochastic-gradient and Semi-gradient Methods
------
SGD: stochastic gradient descent

![](../master/RL_png/image123.png?raw=true)
![](../master/RL_png/image124.png?raw=true)

![](../master/RL_png/image125.png?raw=true)

![](../master/RL_png/image126.png?raw=true)

![](../master/RL_png/image127.png?raw=true)

9.4 Linear Methods
------
![](../master/RL_png/image128.png?raw=true)

![](../master/RL_png/image129.png?raw=true)

![](../master/RL_png/image130.png?raw=true)

![](../master/RL_png/image131.png?raw=true)
![](../master/RL_png/image132.png?raw=true)
![](../master/RL_png/image133.png?raw=true)

![](../master/RL_png/image134.png?raw=true)

![](../master/RL_png/image135.png?raw=true)

9.5 Feature Construction for Linear Methods
------
* 9.5.1 Polynomials
* 9.5.2 Fourier Basis
* 9.5.3 Coarse Coding
* 9.5.4 Tile Coding
* 9.5.5 Radial Basis Functions

9.6 Nonlinear Function Approximation: Artificial Neural Networks
------
![](../master/RL_png/image136.png?raw=true)

![](../master/RL_png/image137.png?raw=true)

hidden layers, backpropagation, Dropout, deep belief networks, CNN

9.7 Least-Squares TD
------
![](../master/RL_png/image138.png?raw=true)
![](../master/RL_png/image139.png?raw=true)

![](../master/RL_png/image140.png?raw=true)

![](../master/RL_png/image141.png?raw=true)

10 On-policy Control with Approximation
======

![](../master/RL_png/image142.png?raw=true)

10.1 Episodic Semi-gradient Control
------
![](../master/RL_png/image143.png?raw=true)

![](../master/RL_png/image144.png?raw=true)

![](../master/RL_png/image145.png?raw=true)

![](../master/RL_png/image146.png?raw=true)

10.2 n-step Semi-gradient Sarsa
------
![](../master/RL_png/image147.png?raw=true)

![](../master/RL_png/image148.png?raw=true)

10.3 Average Reward: A New Problem Setting for Continuing Tasks
------
![](../master/RL_png/image149.png?raw=true)
![](../master/RL_png/image150.png?raw=true)

![](../master/RL_png/image151.png?raw=true)

![](../master/RL_png/image152.png?raw=true)
![](../master/RL_png/image153.png?raw=true)

![](../master/RL_png/image154.png?raw=true)

10.4 Deprecating the Discounted Setting
------
![](../master/RL_png/image155.png?raw=true)

![](../master/RL_png/image156.png?raw=true)

10.5 n-step Differential Semi-gradient Sarsa
------
![](../master/RL_png/image157.png?raw=true)

![](../master/RL_png/image158.png?raw=true)

![](../master/RL_png/image159.png?raw=true)

11 Off-policy Methods with Approximation
======

![](../master/RL_png/image160.png?raw=true)

11.1 Semi-gradient Methods
------
![](../master/RL_png/image161.png?raw=true)

![](../master/RL_png/image162.png?raw=true)

11.3 The Deadly Triad
------
Incomplete

12 Eligibility Traces
=======
![](../master/RL_png/image163.png?raw=true)

12.1 The λ-return
------
![](../master/RL_png/image164.png?raw=true)

![](../master/RL_png/image165.png?raw=true)

![](../master/RL_png/image166.png?raw=true)

![](../master/RL_png/image167.png?raw=true)

![](../master/RL_png/image168.png?raw=true)

![](../master/RL_png/image169.png?raw=true)

![](../master/RL_png/image170.png?raw=true)

12.2 TD(λ)
------
![](../master/RL_png/image171.png?raw=true)

![](../master/RL_png/image172.png?raw=true)

![](../master/RL_png/image173.png?raw=true)

12.3 An On-line Forward View
------
![](../master/RL_png/image174.png?raw=true)

![](../master/RL_png/image175.png?raw=true)

12.4 True Online TD(λ)
------
![](../master/RL_png/image176.png?raw=true)

![](../master/RL_png/image177.png?raw=true)

12.5 Dutch Traces in Monte Carlo Learning
------
Incomplete

13 Policy Gradient Methods
======
![](../master/RL_png/image178.png?raw=true)

13.1 Policy Approximation and its Advantages
------
![](../master/RL_png/image179.png?raw=true)

13.2 The Policy Gradient Theorem
------
![](../master/RL_png/image180.png?raw=true)

![](../master/RL_png/image181.png?raw=true)

![](../master/RL_png/image182.png?raw=true)

13.3 REINFORCE: Monte Carlo Policy Gradient
------
![](../master/RL_png/image183.png?raw=true)

![](../master/RL_png/image184.png?raw=true)

![](../master/RL_png/image185.png?raw=true)

![](../master/RL_png/image186.png?raw=true)

![](../master/RL_png/image187.png?raw=true)

![](../master/RL_png/image188.png?raw=true)

13.4 REINFORCE with Baseline
------
![](../master/RL_png/image189.png?raw=true)

![](../master/RL_png/image190.png?raw=true)

13.5 Actor-Critic Methods
------
![](../master/RL_png/image191.png?raw=true)

![](../master/RL_png/image192.png?raw=true)

![](../master/RL_png/image193.png?raw=true)

13.6 Policy Gradient for Continuing Problems (Average Reward Rate)
------
![](../master/RL_png/image194.png?raw=true)
![](../master/RL_png/image195.png?raw=true)

![](../master/RL_png/image196.png?raw=true)

![](../master/RL_png/image197.png?raw=true)

13.7 Policy Parameterization for Continuous Actions
------
Incomplete

14 Psychology
======

15 Neuroscience
======

16 Applications and Case Studies
======

16.1 TD-Gammon
------

![](../master/RL_png/image198.png?raw=true)

three-ply search

![](../master/RL_png/image199.png?raw=true)

Reference:
* 1995 Temporal difference learning and TD-Gammon.pdf

16.2 Samuel's Checkers Player
------
Reference:
* 1969 Some Studies in Machine Learning Using the Game of Checkers.pdf

16.6 Human-Level Video Game Play
------
DQN, gradient-descent form of Q-learning
* https://sites.google.com/a/deepmind.com/dqn
* https://github.com/Kaixhin/Atari
* https://github.com/songrotek/DQN-Atari-Tensorflow
* 2013.10 Playing Atari with Deep Reinforcement Learning.pdf
* 2015.02 Human-level control through deep reinforcement learning.pdf
* 2014 Deep learning for real-time Atari game play using offline Monte-Carlo tree search planning.pdf
* 2015.10 Deep Reinforcement Learning with Double Q-learning.pdf
* 2016.04 Dueling Network Architectures for Deep Reinforcement Learning.pdf
* 2016.06 Asynchronous Methods for Deep Reinforcement Learning.pdf

16.7 Mastering the Game of Go
------

Reference:
* 2015 Better Computer Go Player with Neural Network and Long-term Prediction.pdf
* 2015 Move Evaluation in Go Using Deep Convolutional Neural Networks.pdf
* 2016 Mastering the Game of Go with Deep Neural Networks and Tree Search.pdf
