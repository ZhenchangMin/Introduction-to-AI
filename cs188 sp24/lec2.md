# Lec2: Search: State Spaces, Uninformed Search
## Agents that Plan
Reflex agents:
- Choose action based on current percept
- May have memory or a model    
- Do not consider the consequences of actions
- Consider how the world **is**

Planning agents:
- Ask "what if"
- Decision based on (hypothetical) consequences of actions
- Formulate a goal
- Consider how the world **would be**

## Search Problems
A `search problem` consists of:
- A state space
- A successor function
- A start state
- A goal test

A `solution` is a sequence of actions (a plan) which transforms the start state to a goal state
![Example](image/lec2/1756949471181.png)

### What's in a State Space
The `world state` includes every last detail of the environment
A `search state` keeps only the details needed for planning (abstraction)
![In a state space](image/lec2/1756949755049.png)

## State Space Graphs
![State space graph](image/lec2/1756949871442.png)

## Search Trees
![Search tree](image/lec2/1756949983197.png)
![1756950396732](image/lec2/1756950396732.png)
fringe: a data structure used to store all the possible states (nodes) that you can go from the current states.
![1756950947652](image/lec2/1756950947652.png)
This algorithm expands nodes and try to generate one path from start state to goal state.
Node is made up with 4 parts:
- State: the current state
- Parent: the state that leads to the current state
- Action: the action that leads to the current state
- Path cost: the cost of the path from the start state to the current state, usually denoted as g(node)

We can use stacks to store frontiers.
- is_empty(frontier)
- pop(): remove the last element in the stack
- add(node): add a node to the stack

## Depth-First Search
