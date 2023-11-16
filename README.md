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
Using a graph theory book I have, "Introduction to Graph Theory by Richard J. Trudeau", he states that 
'an isomorphism is a one-to-one correspondence between vertex sets' and goes on to mention that 'an 
isomorphism induces a one-to-one correspondence between edge sets.' This merely re-states what our formal definition
defines as an isomorphism between graphs, however this definition involving sets makes the proof more straightforward.
\
\
If we have two graphs with the same number of nodes, then we already know we can create a one-to-one mapping of the 
nodes from one graph to another which satisfies part of our isomorphism definition. 
This leaves us with only the edges to worry about, as simply mapping all of the nodes doesn't necessarily mean the graphs 
are isomorphic.
\
\
However since we also know that both graphs are completely connected then we know that both graphs will
have the same number of edges as well, but this also doesn't prove isomorphism as two graphs can have the same number of
nodes and edges but one might have a different circuit length (a path that begins and ends at the same node) which breaks the 
definition of isomorphism as one graph would have an edge that isn't in the edge set of the other after mapping nodes.
\
\
Luckily we can ignore the circuit condition as we're talking about two completely connected graphs, which means that 
both graphs must have the same circuit lengths for every node and thus two completely connected graphs with equal numbers of
nodes must be isomorphic, as there isn't any way to create a one-to-one mapping of nodes that doesn't also follow the 
$(u,v) \in E_1$ iff $(f(u),f(v)) \in E_2$ part of our definition.
