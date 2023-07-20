*This short paper is a project that concludes my first part of IBM Quantum Explorers 2023. I will try to utilize my University knowledge and things that I have learned during this course to present Mathematical foundations of Qbits. I'm going to skip many important topics, for now, but those notes will be extended in time. 
I am opened to any feedback about my work. In order to communicate, please open issue.*

# 101 Math and physics needed to understand how quantum computer works.

## 0. Space definition
### Definition 1: 
Linear space $\mathbb{V}$ ia a set of objects $\\ket{1},\\ket{3},...\\ket{V},...,\\ket{W}...$ named vectors for which exist: 
1) sum noted as $\\ket{V}+\\ket{W}$
2) scalar product of vector and scalar *a,b,...* noted as $a\\ket{V}$

above need to also satisfy few conditions:

- result of any scalar product or sum needs to be part of the same space
- $a(\\ket{V}+\\ket{W}) = a\\ket{V}+a\\ket{W}$
- $(a+b)\\ket{V}=a\\ket{V}+b\\ket{V}$
- $\\ket{V}+\\ket{W}=\\ket{W}+\\ket{V}$
- $\\ket{V}+(\\ket{W}+\\ket{Z}=(\\ket{V}+\\ket{W})+\\ket{Z}$
- there exists zero vector $\\ket{0}$ where $\\ket{V}+\\ket{0}=\\ket{V}$
- for every vector $\\ket{V}$ exists opposite vector $\\ket{-V}$ where $\\ket{V}+\\ket{-V} = \\ket{0}$

  ### Definition 2:
  Set of numbers *a,b,...* is called field over which linear space is defined
  
Let's imagine set $\\ket{1},\\ket{3},...\\ket{N}$ and call it linearly independent if $$\sum_{i=1}^{N} a_i\\ket{i} = \\ket{0}$$ is satisfied only for trivial case, ahere all *a_n* are zero. This implies, that none of the vectors from set of linearly independent cannot be represented as combination of others from this set.


Now let's imagine that we have *N* very small particle detectors setup in the straight line. We send an electron along this line and observe which detector shown a spike. Let's say it was detector *K* that observed our electron. This means that our electron was in state $\\ket{K}$, where K=1,2,...N is base of state space. Note that is detector K observed electron it means that no other did it.
## 1. General rule of superposition
Lets have vector $\overrightarrow{x}$ such as: $$\overrightarrow{x}=x_1\overrightarrow{e_1}+x_2\overrightarrow{e_2}+x_3\overrightarrow{e_3}$$
it can also be represented as:
$$\\ket{x} = x_1\\ket{e_1}+ x_2\\ket{e_2}+x_3\\ket{e_3}$$
So let's generalize this notation to any *N*-dimension vector
$$\\ket{\\psi} = \\psi_1\\ket{1}+ \\psi_2\\ket{2}+\\psi_3\\ket{3}+...+\\psi_N\\ket{N}$$
where $$Dim\ \\psi = N$$
fron now on, we will consider $\\ket{\\psi}$ a state that is a linear combination of all possible states in a given measurement space with probability amplitude $P$ of finding particle in state $i$  $P_i=|\\psi_i|^2$
therefore if $\\ket{\\psi}$ and $\\ket{\\delta}$ are states, then $\\alpha\\ket{\psi} + \\beta\\ket{\\delta}$ are also states hence: $$\\ket{\\psi} = \\sum_{k=1}^N \\psi_k \\ket{K} =  \\sum_{k=1}^N \\Delta \frac{\\psi_k}{\\sqrt\\Delta}\frac{\\ket{k}}{\\sqrt\\Delta}=\\int_0^l dx \\psi(x)\\cdot\\ket{x}$$
where $\\psi(x)$ is wave function and $\\ket{x}$ is element in base of states space of particle.
Having above in mind $\langle{K}|{K}\rangle  = 1$ and $\langle{K}|{L}\rangle = \\delta_kl$
## 2. Probability of measuring particle in state $\\ket{\psi_2}$
We need to first answer question: what is measurement? By measurement we mean projection opeartion that when applied to a state projects one and only one state from possible spectrum. 
Considering location operation, where we want to measure location of particle we use operatior: $\\int \ dx \ {\psi}^\ast_2(x)\psi_1(x)$



