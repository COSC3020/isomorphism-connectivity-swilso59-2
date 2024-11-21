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
- In order to prove this we can use a proof by contradiction.
- $G_{1}$ has vertices $A, B, C$ and one edge $(A, B)$.
- $G_{2}$ has vertices $1, 2, 3$ and one edge $(1, 2)$.
- Neither $G_{1}$ or $G_{2}$ are completely connected.
- If we have a function $f: V_{1} \rightarrow V_{2}$. That maps the vertices and edges form $G_{1}$ to $G_{2}$ such as $f(A) = 1, f(B) = 2, f(C) = 3$.
- We can look at the correcsponding nodes and edges to check if the to determine if the graph holds the same structure.
- In $G_{1}, (A, B) \in E_{1}$. $f$ maps to $f(A), f(B) = (1, 2) \in E_{2}$.
  - The non-edge in $G_{1}$, between $A$ and $C$. Maps to no edge between $f(A) = 1, f(C) = 3$ in $G_{2}$.
- from here we can see that all edges and non-edges in $G_{1}$ maintain the structue when mapped to the edges and non-edges in $G_{2}$.
- This satisfies the isomorphism condition.

Counter-example:
- If we have two graphs $H_{1}$ and $H_{2}$.
  - $H_{1}$ has 3 vertices $(A, B, C)$ and one edge $(A, B)$.
  - $H_{2}$ has 3 vertices $(1, 2, 3, 4)$ and two edges $(1, 2)$ and $(3,4)$.
- $H_{1}$ has 3 vertices $(A, B, C)$.
- $H_{2}$ has 4 vertices $(1, 2, 3, 4)$.
- There is no one-to-one and onto mapping between $H_{1}$ and $H_{2}$.
- There is no vertex in $H_{1}$ that can correspond to 4 in $H_{2}$.
- This violates the bijection requirement.
  - There are more vertices in $H_{2}$ than in $H_{1}$. This makes it impossible for every vertex in $H_{2}$ to be mapped to by a vertex in $H_{1}$.
  - If you assign $A, B, C$ to multiple vertices you will break the one-to-one condition as well.
 
For this assignment I reviewed the repository from https://github.com/COSC3020/isomorphism-connectivity-Dhruv8806 and https://github.com/COSC3020/isomorphism-connectivity-DJReflexive. This is where I got the idea to providing a counter example from. 

“I certify that I have listed all sources used to complete this exercise, including the use
of any Large Language Models. All of the work is my own, except where stated
otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is
suspected, charges may be filed against me without prior notice.”
