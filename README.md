# Graph-Partitioning-for-VLSI-using-DSA

The graph partitioning problem is that of dividing the vertices of a graph into sets of speci ed sizes such that few edges cross between sets. This NP{complete problem arises in many important scienti c and engineering problems. Prominent examples include the decomposition of data structures for parallel computation, the placement of circuit elements and the ordering of sparse matrix computations. We present a multilevel algorithm for graph partitioning in which the graph is approximated by a sequence of increasingly smaller graphs. The smallest graph is then partitioned using a spectral method, and this partition is propagated back through the hierarchy of graphs. A variant of the Kernighan-Lin algorithm is applied periodically to re ne the partition. The entire algorithm can be implemented to execute in time proportional to the size of the original graph. Experiments indicate that, relative to other advanced methods, the multilevel algorithm produces high quality partitions at low cost. 

Move-based iterative improvement partitioning methods such as the Fiduccia- Mattheyses (FM) algorithm and Krishnamurthy's Look-Ahead (LA) algorithm are widely used in VLSI CAD applications largely due to their time efficiency and ease of implementation. This class of algorithms is of the "local improvement" type. They generate relatively high quality results for small and medium size circuits. However, as VLSI circuits become larger, these algorithms are not so effective on them as direct partitioning tools. We propose new iterative-improvement methods that select cells to move with a view to moving clusters that straddle the two subsets of a partition into one of the subsets. The new algorithms significantly improve partition quality while preserving the advantage of time efficiency. Experimental results on 25 medium to large size ACM/SIGDA benchmark circuits show up to 70% improvement over FM in cutsize, with an average of per-circuit percent improvements of about 25%, and a total cut improvement of about 35%. They also outperform the recent placement-based partitioning tool Paraboli and the spectral partitioner MELO by about 17% and 23%, respectively, with less CPU time. This demonstrates the potential of iterative improvement algorithms in dealing with the increasing complexity of modern VLSI circuitry.


Input format:

7 5

3 1 0 4

3 3 2 0

3 3 2 1

2 5 2

2 6 3

3 4

The first number of the first line (7) indicates how many nodes or vertices are in the graph of the input.

The second number of the first line (5) indicates how many edges are in the graph of the input.

The subsequent lines are for each of the edges.

The first number of each subsequent line (3 of line 2 and so on) is the number of nodes or vertices are in the edge (since the partitioning and the placement support hyper edges). However, if you want to run the Routing file, make sure all of the edges only contain two nodes or vertices.

The following numbers are the node indexes. They don't need to be in any order or start at any number at all.

The last line is the constraints for the partition file. The first number (3) is the minimum of the smaller partition.
