# Graph-Size-Estimation-with-Random-Walks
Applied Mathematics

Explanation for non-French speakers:

Given a finite, undirected and connected graph 𝐺=(𝑉,𝐸), we seek to estimate its size. Suppose we access the graph in the following way: we can access a particular vertex of the graph, and having accessed a vertex 𝑖 of the graph, we can then access any neighbor 𝑗 of 𝑖 in 𝐺 .

We will consider the following algorithm for estimating this size: We set a length τ , and a target number ℓ . At each step 𝑡≥1 , we construct a random walk of length τ , that is: 𝑋𝑡0,...,𝑋𝑡τ on the graph, resulting from 𝑋𝑡0=𝑖0 . By definition, given the choices 𝑋𝑡0,...,𝑋𝑡𝑠−1, 𝑋𝑡𝑠 is uniformly randomly selected among the neighbors of 𝑋𝑡𝑠−1 in 𝐺 . We denote by 𝑌𝑡=𝑋𝑡τ the last vertex obtained at the 𝑡-th random walk.

We say we have a collision at step 𝑡 if 𝑌𝑡∈ { 𝑌1,...,𝑌𝑡−1 } =𝐾𝑡 . We note 𝐶ℓ the instant of the ℓ -th collision. The theoretical part establishes theoretical guarantees on the estimation of the number of vertices in the graph. The simulation part consists in the implementation of the described algorithm.
