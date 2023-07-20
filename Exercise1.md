*This short paper is a project that concludes my first part of IBM Quantum Explorers 2023. I will try to utilize my University knowledge and things that I have learned during this course to present Mathematical foundations of Qbits. 
I am opened to any feedback about my work. In order to communicate, please open issue.*

## 101 Math for Qbits

### 0. Space definition
Definition 1: 
Linear space $\mathbb{V}$ ia a set of objects $\\ket{1},\\ket{3},...\\ket{V},...,\\ket{W}...$ named vectors for which exist: 
1) sum noted as follows $\\ket{V}+\\ket{W}$
2) scalar product of vector and scalar *a,b,...* noted as follows $a\\ket{V}$
above need to also satisfy few conditions:
a) result of any scalar product or sum needs to be part of the same space
b) $a(\\ket{V}+\\ket{W}) = a\\ket{V}+a\\ket{W}$
c) $

Let's imagine that we have *N* very small particle detectors setup in the straight line. We send an electron along this line and observe which detector shown a spike. Let's say it was detector *K* that observed our electron. This means that our electron was in state $\\ket{K}$, where K=1,2,...N is base of state space. Note that is detector K observed electron it means that no other did it.
### 1. General rule of superposition
Lets have vector $\overrightarrow{x}$ such as: $$\overrightarrow{x}=x_1\overrightarrow{e_1}+x_2\overrightarrow{e_2}+x_3\overrightarrow{e_3}$$
it can also be represented as:
$$\\ket{x} = x_1\\ket{e_1}+ x_2\\ket{e_2}+x_3\\ket{e_3}$$
So let's generalize this notation to any *N*-dimension vector
$$\\ket{\\psi} = \\psi_1\\ket{1}+ \\psi_2\\ket{2}+\\psi_3\\ket{3}+...+\\psi_N\\ket{N}$$
where $$Dim\ \\psi = N$$
