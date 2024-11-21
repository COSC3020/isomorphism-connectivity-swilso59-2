# Isomorphism

Prove that if two graphs $A$ and $B$ are isomorphic they do *not* have to
be completely connected. I have started with the formal definition of
isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

## Answer 
Example:
- Based on the definition of isomorphism this means that the structure of the edges and non-edges is mainstained under the maping of $f$.
- In order to prove this we can use a direct proof by explicitly verifying the conditions for isomorphism.
- $G_{1}$ has vertices $A, B, C$ and one edge $(A, B)$.
- $G_{2}$ has vertices $1, 2, 3$ and one edge $(1, 2)$.
- Neither $G_{1}$ or $G_{2}$ are completely connected.
- If we have a function $f: V_{1} \rightarrow V_{2}$. That maps the vertices and edges form $G_{1}$ to $G_{2}$ such as $f(A) = 1, f(B) = 2, f(C) = 3$.
- We can look at the correcsponding nodes and edges to check if the to determine if the graph holds the same structure.
- In $G_{1}, (A, B) \in E_{1}$. $f$ maps to $f(A), f(B) = (1, 2) \in E_{2}$.
  - The non-edge in $G_{1}$, between $A$ and $C$. Maps to no edge between $f(A) = 1, f(C) = 3$ in $G_{2}$.
- from here we can see that all edges and non-edges in $G_{1}$ maintain the structue when mapped to the edges and non-edges in $G_{2}$.
- This satisfies the isomorphism condition.
 
For this assignment I reviewed the repository from https://github.com/COSC3020/isomorphism-connectivity-Dhruv8806 and https://github.com/COSC3020/isomorphism-connectivity-DJReflexive. 

“I certify that I have listed all sources used to complete this exercise, including the use
of any Large Language Models. All of the work is my own, except where stated
otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is
suspected, charges may be filed against me without prior notice.”
