# Co-Operation-in-Ad-hoc-networks-a-machine-learning-ap
Reinforcement learning technique is used to discover the optimum path while relaying the packets from source node to destination node.

## Reinforcement Learning:

    Reinforcement learning is learning what to do how to map situations to actions so as to maximize a numerical reward signal. The learner is not told which actions to take, as in most forms of machine learning, but instead must discover which actions yield the most reward by trying them.
	 Reinforcement learning is defined not by characterizing learning methods, but by characterizing a learning problem. Any method that is well suited to solving that problem, we consider to be a reinforcement learning method.
  The basic idea is simply to capture the most important aspects of the real problem facing a learning agent interacting with its environment to achieve a goal. Clearly, such an agent must be able to sense the state of the environment to some extent and must be able to take actions that affect the state. The agent also must have a goal or goals relating to the state of the environment. The formulation is intended to include just these three aspects sensation, action, and goal in their simplest possible forms without trivializing any of them.
  
## Q-Learning algorithm:
  
> Q-Learning algorithm is used to implement Reinforcement Learning in Ad-Hoc network. 
> The transition rule of Q learning is a very simple formula:
  Q(state, action) = R(state, action) + Gamma * Max[Q(next state, all actions)]
> According to this formula, a value assigned to a specific element of matrix Q, is equal to the sum of the corresponding value in matrix R and the learning parameter Gamma, multiplied by the maximum value of Q for all possible actions in the next state. 

### The Q-Learning algorithm goes as follows:

> set the gamma parameter and environment rewards in matrix R.
> Initialize matrix Q to zero.
> For each episode: Select a random initial state.
  Do while the goal state hasn't been reached.
  Select one among all possible actions for the current state.
  Using this possible action, consider going to the next state.
  Get maximum Q value for this next state based on all possible actions.
  Compute: Q(state, action) = R(state, action) + Gamma * Max[Q(next state, all actions)]
  Set the next state as the current state.
  End Do
End For

### Algorithm to utilize the Q matrix

> Set current state = initial state.
> From current state, find the action with the highest Q value.
> Set current state = next state.
> Repeat Steps 2 and 3 until current state = goal state.
> The algorithm above will return the sequence of states from the initial state to the goal state.

## Example with explanation:

> Suppose we have Eleven nodes [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10 and 11] are arranged and rewards are assigned to each link between the nodes. Links which are attached to destination node that is 10 assigned by reward 100, nodes which are just connected that link assigned zero and nodes which are not connected are assigned by reward -1 as follows.

> This R_Table is provided to Brain of agent which will help in calculating the corresponding Q value. The path which possess maximum Q value that path have to be choose which is optimum path. Initially Q values assign with zero.

> ![screenshot 839](https://user-images.githubusercontent.com/32256364/42685099-bb11f306-86af-11e8-97e6-16449b83e048.png)



