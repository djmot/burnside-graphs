# burnside-graphs

B(m,n) is defined to be the largest group with m generators and exponent n:

$B(m,n) = \langle x_1, ... , x_m | g^n = 1 \forall g \rangle$

This program computes the Cayley graph of the above presentation for the groups B(2,n). 

It uses a heuristic method of iteratively extending then pruning the graph.

New paths are added in such a way that relations of the form $g^n = 1$ are likely to result in pruning nodes later on in the process.

The program successfully computes B(2,n) for $n = 2, 3, 4$. It's unknown if B(2,5) is finite; if it is finite, it's too large to be computed in this way. Further, there is no guarantee that this program will be able to compute the graph even given infinite time and memory.
