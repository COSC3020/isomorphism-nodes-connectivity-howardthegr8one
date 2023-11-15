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
$A$ and $B$ are isomorphic. Using proof by contrapositive our new logical statement becomes $\neg R \rightarrow (\neg P \lor \neg Q)$
\
\
Let $A$ and $B$ be two graphs who are NOT isomorphic. If the graphs aren't isomorphic then $A$ and $B$ do not have the same 
number of nodes or $A$ and $B$ are not completely connected. Not being isomorphic means that there does not exist a one-to-one 
and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v) \in E_1$ iff $(f(u),f(v)) \in E_2$. 
\
\
Case 1: $|A| \neq |B|$ \
If graphs $A$ and $B$ don't have the same number of nodes then a bijection function isn't possible. This is because if $|A| \neq |B|$ 
then $|A| < |B|$ or $|A| > |B|$, and in either case a one-to-one mapping can't happen as all of the nodes of $A$ will be mapped but nodes 
in $B$ won't be mapped to anything, or vice versa which prevents a one-to-one mapping. Therefore when $|A| \neq |B|$ the graphs can't be 
isomorphic.
\
\
Case 2: $A \wedge B$ are not completely connected \
If graphs $A \wedge B$ are not completely connected then one can be completely connected while the other isn't, or vice versa, or neither 
can be completely connected. In any of these three cases, even if the graphs have equal numbers of nodes, there isn't a guarantee that they 
will have the same number of edges. In fact in the case that only one of the graphs is completely connected then a bijection mapping isn't 
possible because there will be at least one instance where $(u,v) \in E_1$ but $(f(u), f(v)) \notin E_2$ which goes against our definition of 
isomorphism. We also can't say that two graphs in which are neither completely connected can be isomorphic as it would depend on the specifics
of the given graphs. Therefore $A$ and $B$ aren't isomorphic when $A \wedge B$ are not completely connected. 
\
\
Thus by directly proving the contrapositive of our statement we have proven the original statement that "If $A$ and $B$ have the same number of 
nodes and are both completely connected then $A$ and $B$ are isomorphic"
