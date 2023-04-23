# Graph Theory Cheatsheet

## Graph Types

1. **Undirected Graph**: A graph with edges that have no direction.
2. **Directed Graph (Digraph)**: A graph with edges that have a direction.
3. **Weighted Graph**: A graph with a weight (value) associated with each edge.
4. **Unweighted Graph**: A graph without weights associated with edges.
5. **Cyclic Graph**: A graph containing at least one graph cycle.
6. **Acyclic Graph**: A graph with no cycles.
7. **Connected Graph**: A graph where there is a path between every pair of vertices.
8. **Disconnected Graph**: A graph where some vertices are not connected by any path.
9. **Complete Graph**: A graph where there is an edge between every pair of vertices.
10. **Bipartite Graph**: A graph where its vertices can be divided into two disjoint sets such that every edge connects vertices from different sets.
11. **Planar Graph**: A graph that can be drawn on a plane without any edge crossings.
12. **Tree**: An acyclic, connected, undirected graph.

## Graph Formulas and Concepts

### Degree

- **Degree of a vertex (deg(v))**: The number of edges incident to the vertex.
- **In-degree (indeg(v))**: In a directed graph, the number of edges coming into the vertex.
- **Out-degree (outdeg(v))**: In a directed graph, the number of edges going out from the vertex.

### Handshaking Lemma

- In an undirected graph, the sum of the degrees of all vertices is equal to twice the number of edges.

`∑ deg(v) = 2 * |E|`

### Euler's Formula

- For a connected planar graph with |V| vertices, |E| edges, and |F| faces:

`|V| - |E| + |F| = 2`

### Graph Connectivity

- **Connected Components**: Subgraphs where each vertex is connected to every other vertex in the subgraph.
- **Strongly Connected Components (SCCs)**: In a directed graph, subgraphs where there is a directed path between every pair of vertices.
- **Weakly Connected Components (WCCs)**: In a directed graph, subgraphs obtained by replacing all directed edges with undirected edges.

### Graph Isomorphism

Two graphs G1 and G2 are isomorphic if there is a one-to-one correspondence between their vertices and edges that preserves adjacency.

### Graph Representation

1. **Adjacency Matrix**: A matrix A of size |V| x |V|, where A[i][j] = 1 if there's an edge between vertices i and j, and A[i][j] = 0 otherwise.
2. **Adjacency List**: An array of lists, where the list at index i contains the neighbors of vertex i.

## Graph Algorithms

1. **Breadth-First Search (BFS)**: A graph traversal algorithm that visits all vertices reachable from a given source vertex in breadth-first order.
2. **Depth-First Search (DFS)**: A graph traversal algorithm that visits all vertices reachable from a given source vertex in depth-first order.
3. **Dijkstra's Algorithm**: A shortest-path algorithm for non-negative weighted graphs.
4. **Bellman-Ford Algorithm**: A shortest-path algorithm for graphs with negative weights and without negative cycles.
5. **Floyd-Warshall Algorithm**: An all-pairs shortest-path algorithm for weighted graphs.
6. **Kruskal's Algorithm**: A minimum spanning tree algorithm for undirected, weighted graphs.
7. **Prim's Algorithm**: Another minimum spanning tree algorithm for undirected, weighted graphs.
8. **Topological Sort**: A linear ordering of the vertices of a directed acyclic graph (DAG) such that for every directed edge (u, v), vertex u comes before vertex v in the ordering.
9. **Maximum Flow**: Algorithms for finding the maximum flow in a flow network (e.g., Ford-Fulkerson, Edmonds-Karp).

Remember, this is a basic cheatsheet and does not cover every aspect of graph theory. It's meant to serve as a quick reference for important concepts, formulas, and algorithms.
