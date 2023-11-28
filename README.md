[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=12837089&assignment_repo_type=AssignmentRepo)
# Isomorphism

Prove that if two graphs $A$ and $B$ have the same number of nodes and are
completely connected, they must be isomorphic. I have started with the formal
definition of isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.


# My Proof: 
Using induction let's establish a base case where we have two graphs, $A$ and $B$, that both have a single node each and are
completely connected. Since they both only have a single node then neither graph will have any edges as the sole node in the 
graphs don't have any other node to connect to. Since we can obviously map the sole node in $A$ to the sole node in $B$ and 
we have no edges to worry about then this mapping would be a bijection and thus the two graphs are isomorphic. 
\
\
Let $P(n)$ be the statement that two complete graphs, $A$ and $B$ have the same $n$ number of nodes and are isomorphic. We've 
already explained how this is true for $n = 1$. Let n = k. Since we know $P(k)$ is true for our base case where $k = 1$, 
now we must show that $P(k+1)$ is also true. 
\
\
By adding a single node to both of our graphs and keeping them completely connected, our graphs would now have two nodes each, 
additionally we would have to add a single edge to connect these two nodes for each graph. Each graph now has two nodes connected
by a single edge. If we simply map the new node in one graph to the new node in the other graph then we know we still have a 1-to-1
mapping of the nodes, furthermore since we only have a single edge to worry about in both graphs, and the nodes are already mapped
then the mapping function would have to map the single edge in one graph to the sole edge in the other graph, which maintains our
isomorphism between graphs. 
\
\
Adding a single node to a given graph that is completely connected will always result in adding $V$ edges
to the graph as well, where $V$ is the number of nodes in the graph before adding the new one. This is always true as the new node must
connect to every other node in the graph, thus adding a node to a graph with $V$ nodes and $E$ edges results in the graph gaining $V$ edges.
Since our original $P(k)$ statement is true for our base case, and because it's true for $k+1$ then by induction we've shown that two graphs
which have the same number of nodes and are completely connected are always isomorphic.
