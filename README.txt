Q1)
In DepthFirstSearch, we utilize the data structure of a stack since it is a Last In First Out structure.
First push the start state and path onto the stack, then pop off a vertex. If current state is the goal
state, then return directions immediately. If a state has not been visited, then add to visited list and
explore its adjacent successors by pushing onto stack.

Q2)
BreadthFirstSearch is very similiar to DepthFirstSearch, but instead explores the first vertexes present
instead of exploring to the deepest first. To implement this function, we will instead use a Queue
data structure since it is a First in First Out struture.

Q3)
UniformCostSearch uses a PriorityQueue instead of a regular Queue like in BFS, because it needs to keep 
the cost of each state. Also, instead of using a list for visited vertexes, it is replaced by a dictionary
to keep track of the cost as well. The overall structure of the code if very similiar to DFS and BFS.

Q4)
A* Search also uses a PriorityQueue just like the UniformCostSearch, but the main difference is the cost
calculated from heuristic function. This time when exploring unvisited vertexes, will update the heuristic
cost of the new state and update the priority queue.
