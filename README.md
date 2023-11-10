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
"If $A$ and $B$ have the same number of nodes and are both completely connected then $A$ and $B$ are isomorphic" 
can be written in the form $(P \wedge Q) \rightarrow R$ where $P$ is the statement $A$ and $B$ have the same 
number of nodes, $Q$ is the statement that $A$ and $B$ are completely connected graphs, and $R$ is the statement 
$A$ and $B$ are isomorphic. Using proof by contradiction our new logical statement becomes $(P \wedge Q) \rightarrow \neg R$
\
\
Let $A$ and $B$ be two graphs who have the same number of nodes, are completely connected, and are NOT isomorphic. 
Not being isomorphic means that there does not exist a one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such 
that $(u,v) \in E_1$ iff $(f(u),f(v)) \in E_2$. However since $A$ and $B$ have the same number of nodes then we can at 
minimum map every node in $A$ to one and only one node in $B$. 
\
\
Since every node in both graphs can be mapped to one and only one node in the other graph and since the graphs are completely 
connected it would mean that all nodes in both graphs will have corresponding degrees then the mapping would be a bijection, 
which contradicts our statement that two graphs who share the same number of nodes and are completely connected are NOT isomorphic. 
This contradiction proves our original statement that if $A$ and $B$ have the same number of nodes and are both completely connected 
then $A$ and $B$ are isomorphic.
