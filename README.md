# lca
Quick lowest-common-ancestor queries using sparse tables. The function lca(x,y) takes two node identifiers in a rooted tree and returns their lowest common ancestor. The function takes `O(lg N)` time where `N` is the number of nodes in the tree. A `O(N lg N)` pre-processing step is needed.

# API
* void init( void ); // Initialize the module (assumes that the tree is built and the number of nodes is stored in variable n
* void lca(int x, int y) // Lowest common ancestor of x and y
