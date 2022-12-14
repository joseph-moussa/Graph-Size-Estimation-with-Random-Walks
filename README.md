# Graph-Size-Estimation-with-Random-Walks
Applied Mathematics Project at Γcole Polytechnique

Explanation for non-French speakers:

Given a finite, undirected and connected graph πΊ=(π,πΈ), we seek to estimate its size. Suppose we access the graph in the following way: we can access a particular vertex of the graph, and having accessed a vertex π of the graph, we can then access any neighbor π of π in πΊ .

We will consider the following algorithm for estimating this size: We set a length Ο , and a target number β . At each step π‘β₯1 , we construct a random walk of length Ο , that is: ππ‘0,...,ππ‘Ο on the graph, resulting from ππ‘0=π0 . By definition, given the choices ππ‘0,...,ππ‘π β1, ππ‘π  is uniformly randomly selected among the neighbors of ππ‘π β1 in πΊ . We denote by ππ‘=ππ‘Ο the last vertex obtained at the π‘-th random walk.

We say we have a collision at step π‘ if ππ‘β { π1,...,ππ‘β1 } =πΎπ‘ . We note πΆβ the instant of the β -th collision. The theoretical part establishes theoretical guarantees on the estimation of the number of vertices in the graph. The simulation part consists in the implementation of the described algorithm.
