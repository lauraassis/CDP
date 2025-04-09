# CDP
# Capacitated Districting Problem (CDP) 

###########################################################
# This repository provides information about 24 types of 
# instances to the CDP, and for each type, there are 10 
# networks. Besides, a large real network is given as well, 
# consisting of 241 instances for the CDP.
# By:
# 1. Laura Assis - laura.assis@cefet-rj.br
# 2. Fábio Usbertti - fusberti@ic.unicamp.br
# 3. Paulo França - paulo.morelato@gmail.com
# 4. Augusto Mendonça - augusto01@gmail.com
###########################################################

Explanation of Instances:

The instances are 24 randomly generated type of networks, classified using the following taxonomy (doi: http://dx.doi.org/10.1016/j.cor.2013.08.002):

- Group: 512 nodes (A) or 1024 nodes (B);

- Family: Demand 1 (reading time, in minutes), uniformly distributed within a tight range [16, 24](1) or within a loose range[12, 28](2);

- Class: Demand 2 (number of customers), uniformly distributed within a tight range [160, 240](1) or a loose range [120, 280](2);

- Sparsity: full grid (00), sparse grid (25) and spanning tree (50).

Geographical coordinates were set so that the networks turn up into grids. Some minor disturbances in the coordinates were employed to avoid symmetry.


Input Format:

n - number of nodes
m - number of edges 
P - number of districts 
tau - tolerance for district capacity violation, which can be an external parameter

A list of size n, with information about the nodes containing:
- x and y coordinates of node i
- The original district that node i is assigned to

A list of size m, with information about the edges containing:
- Node i adjacent to node j (edje e)
- number of customers (or number of electric meters) 
- reading time  

