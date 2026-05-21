Theoretical Foundations of Reinforcement Learning: From Bellman Equations to Deep RL Algorithms
============================================================================================

Overview
--------
This Summer of Code plan aligns week-by-week with David Silver's RL lectures and builds from
core theory to modern deep RL. Each week has topics, resources, and deliverables. The final
two weeks focus on implementing and evaluating selected algorithms from scratch.

Final Component
---------------
In the last two weeks, mentees will work on a mini-project implementing selected RL
algorithms from scratch, bridging theoretical understanding with practical implementation
and empirical evaluation.

Week-by-Week Plan
-----------------

Week 1: Introduction to RL (Lecture 1)
-------------------------------------
Topics
- Agent-environment interaction, return, policies, value functions
- Exploration vs exploitation (high-level intuition)
- Formalizing RL problems as optimization

Resources
- David Silver Lecture 1: https://youtube.com/playlist?list=PLzuuYNsE1EZAXYR4FJ75jcJseBmo4KQ9-&si=f71naScldk1Mbfwi
- Sutton and Barto (2020), Ch. 1: http://incompleteideas.net/book/RLbook2020.pdf
- OpenAI Spinning Up: https://spinningup.openai.com/en/latest/spinningup/rl_intro.html

Deliverables
- 1-2 page write-up defining RL, return, policy, value function, and exploration vs exploitation

Week 2: Algorithm Overview + MDPs (Lectures 1-2)
------------------------------------------------
Topics
- Q-learning and Monte Carlo methods
- Proximal Policy Optimization (PPO)
- Deep Deterministic Policy Gradient (DDPG)
- Soft Actor-Critic (SAC)
- Deep Q-Network (optional)
- MDPs: (S, A, P, R, gamma), Markov property, policies
- State-value and action-value functions

Resources
- David Silver Lectures 1-2: playlist link above
- Sutton and Barto (2020), Ch. 2-3
- OpenAI Spinning Up (for PPO, DDPG, SAC): https://spinningup.openai.com/en/latest/index.html
- OpenAI Spinning Up RL Intro (complete all three parts): https://spinningup.openai.com/en/latest/spinningup/rl_intro.html
- GeeksforGeeks (Q-learning, Monte Carlo): https://www.geeksforgeeks.org/q-learning-in-python/ and https://www.geeksforgeeks.org/monte-carlo-methods-in-reinforcement-learning/
- CS747 (IITB) Section 2 (MDPs): https://www.cse.iitb.ac.in/~shivaram/teaching/old/cs747-s2025/index.html

Deliverables
- A brief report on Q-learning, Monte Carlo, PPO, DDPG, SAC (and optional DQN)
- A glossary that explains all new vocabulary you used in the report
- Short derivation of Bellman expectation equations for V and Q

Important Notes
- Set up dependencies for Spinning Up (needed for Week 5 onward) and start exploring the library
- Start working with OpenAI Gym (or Gymnasium) environments

Week 3: Dynamic Programming + Model-Free Prediction (Lectures 3-4)
------------------------------------------------------------------
Topics
- Bellman expectation and optimality equations
- Policy evaluation, policy iteration, value iteration
- Convergence intuition
- Monte Carlo vs TD learning
- TD(0), TD(lambda)
- Bias-variance tradeoff

Resources
- David Silver Lectures 3-4: playlist link above
- Sutton and Barto (2020), Ch. 4-6

Deliverables
- Pseudocode for policy evaluation, policy iteration, and value iteration
- Compare MC and TD on a small toy MDP (math only)

Week 4: Model-Free Control (Lecture 5)
--------------------------------------
Topics
- SARSA vs Q-learning
- On-policy vs off-policy learning
- Convergence intuition

Resources
- David Silver Lecture 5: playlist link above
- Sutton and Barto (2020), Ch. 6-7

Deliverables
- Derivation and comparison of SARSA and Q-learning updates

Week 5: Value Function Approximation (Lecture 6)
------------------------------------------------
Topics
- Function approximation in RL
- Linear vs nonlinear approximators
- DQN and stability tricks (target networks, replay buffer)

Resources
- David Silver Lecture 6: playlist link above
- Sutton and Barto (2020), Ch. 9
- DQN paper (Nature 2015): https://www.nature.com/articles/nature14236

Deliverables
- Write the DQN loss and explain why replay and target networks help

Week 6: Policy Gradient Methods (Lecture 7)
-------------------------------------------
Topics
- Policy Gradient Theorem (full derivation)
- REINFORCE algorithm
- Variance reduction with baselines

Resources
- David Silver Lecture 7: playlist link above
- Sutton and Barto (2020), Ch. 13
- Spinning Up policy gradient intro: https://spinningup.openai.com/en/latest/spinningup/rl_intro3.html

Deliverables
- Derive REINFORCE with baseline and explain variance reduction

Week 7: Planning, Exploration, and Advanced RL (Lectures 8-10)
--------------------------------------------------------------
Topics
- Model-based RL
- Dyna-Q framework
- Planning vs learning tradeoff
- Epsilon-greedy and softmax exploration
- Upper Confidence Bound (UCB)
- Regret minimization concepts
- Exploration challenges in deep RL
- Limitations of classical RL
- Scaling to complex environments
- Actor-Critic methods, PPO, DDPG, SAC
- Connecting classical RL to deep RL

Resources
- David Silver Lectures 8-10: playlist link above
- Sutton and Barto (2020), Ch. 2 and Ch. 8
- CS747 (IITB) Section 3 (RL): https://www.cse.iitb.ac.in/~shivaram/teaching/old/cs747-s2025/index.html
- Spinning Up (PPO, DDPG, SAC): https://spinningup.openai.com/en/latest/index.html
- PPO paper: https://arxiv.org/abs/1707.06347
- DDPG paper: https://arxiv.org/abs/1509.02971
- SAC paper: https://arxiv.org/abs/1801.01290

Deliverables
- Explain Dyna-Q and compare epsilon-greedy vs UCB
- Summarize strengths and weaknesses of PPO, DDPG, SAC in 1-2 pages

Week 8: Final Project Part 1
----------------------------
Focus
- Choose 1-2 algorithms (e.g., DQN, PPO, SAC)
- Implement from scratch
- Validate math-to-code mapping

Resources
- Spinning Up: https://spinningup.openai.com/en/latest/index.html
- OpenAI Gym: https://www.gymlibrary.dev/ (Gymnasium if preferred)

Deliverables
- Working baseline implementation and initial results

Week 9: Final Project Part 2
----------------------------
Focus
- Run experiments and compare methods
- Document results and insights

Resources
- Sutton and Barto (2020) for theory cross-checks
- Spinning Up and original papers for algorithm details

Deliverables
- Final report and presentation with derivations, implementation notes, and observations

Optional Deep Math Track
------------------------
If you want a more mathematical route, CS747 lectures are excellent. Skip Section 1 (MABs),
build MDP intuition from Section 2, and then cover Section 3 (RL).

CS747 (IITB): https://www.cse.iitb.ac.in/~shivaram/teaching/old/cs747-s2025/index.html
