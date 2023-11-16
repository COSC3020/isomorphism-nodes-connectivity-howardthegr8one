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
Using induction let's establish a base case where we have two graphs, $A$ and $B$ that both have two nodes each and are
completely connected. Since the smallest a complete graph can be is a pair of nodes that connected by a single edge, it is
obvious that these two graphs are isomorphic since we can create a bijection mapping of one graph to the other.
\
\
Let P(n) be the statement that two complete graphs, $A$ and $B$ have the same $n$ number of nodes and are isomorphic. We've 
already explained how this is true for $n = 2$. Let's let n = k. Since we know P(k) is true for our base case where k = 2, 
now we must show that P(k+1) is also true. 
\
\
By adding a single node to both of our graphs and keeping them completely connected, our graphs would now have three nodes each, 
where each node is connected by two edges. Since both graphs increase in size by the same number of nodes and the same number of
edges then we are still able to create a bijection mapping of A to B or vice versa. Adding more nodes won't affect the graphs' 
isomorphism as their sizes will increase simultaneously always allowing for the new nodes/edges to be mapped and retain the bijection
of our mapping from the base case. 
