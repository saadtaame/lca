# lca
Quick lowest-common-ancestor queries using sparse tables. The function `lca(x,y)` takes two node identifiers in a rooted tree and returns their lowest common ancestor (LCA for short). The function takes `O(lg N)` time where `N` is the number of nodes in the tree. A `O(N lg N)` pre-processing step is needed to build the sparse table.

# API
* `void init( void ); // Initialize the module (assumes that the tree is built and the number of nodes is stored in variable n`
* `void lca(int x, int y) // Lowest common ancestor of x and y`

# Other uses
This data structure can also be used to quickly answer path-queries in a (weighted) rooted tree. Examples include sum:
* Find min/max edge weight on path from node x to node y.
* Find weight of path from node x to node y.

The data structure can support updates by adding a function to update the sparse table. An update can be implemented in tim `O(lg N)` so both operations are fast.
