# Isomorphism

Prove that if two graphs $A$ and $B$ do not have the same number of nodes, they
cannot be isomorphic. I have started with the formal definition of isomorphism
below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

A function $f: V_1 \rightarrow V_2$ is onto iff $\forall v_2, \exists v_1, (v_2 \in V_2 \implies v_2 = f(v_1))$

A function $f: V_1 \rightarrow V_2$ is one-to-one iff $f(v_1) = f(v_2) \implies v_1 = v_2$

Proof:

Let there exist two arbitary sets, $S$ and $T$, such that $|S| \neq |T|$. 

Without loss of generality, we can say that $|S| = |T| \pm n$, where $n$ is 
some positive integer. 

Let there exist a function $f: S \rightarrow T$. 

If $f$ were a bijection, then each element in $S$ could be mapped by $f$ to 
some unique element in $T$, and likewise, every element in $T$ would be mapped 
onto by some unique element in $S$, as this is what it means for a function to 
be a bijection. 

However, this cannot occur as there will always be either $n$ elements that 
cannot be mapped to an element in $T$ that has not already been mapped onto, or 
there would be $n$ elements in $T$ that can't be mapped to without mapping multiple 
elements in $S$ to them. If either of these is true, then $f$ cannot be a bijection. 

Therefore, if $A = (V_1 , E_1)$ and $B = (V_2, E_2)$ and $|V_1| \neq |V_2|$, there 
cannot exist a one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ 
such that $(u,v) \in E_1$ iff $(f(u),f(v)) \in E_2$, meaning that $A$ and $B$ 
cannot be isomorphic. 

Q.E.D. 

"I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. 
All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that 
if plagiarism is suspected, charges may be filed against me without prior notice."
