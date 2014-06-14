<a name="graph" />
# Graph
We use `T.Graph` in `t.graph.js` to help implementations of some algorithms in `Graph` static object, which has been put in `graph.*.js`.

All the following methods are call by `Graph.*`. To create a graph object, use `new T.Graph*()` (see [APIType](APIType#graph)).

## Static
Call | Meaning
:----|:-------
`bfs(graph): []` | gets the vertex visiting array by `BFS` order
`dfs(graph): []` | gets the vertex visiting array by `DFS` order
`dijkstra(graph,` <br /> ` s: number = 1): []` | gets the shortest path length of each vertex from initial vertex s
`multiMinimumCut(` <br /> `graph,` <br /> ` times: number): number` | gets the minimum cut number of graph after that times calculations
`mstPrim(` <br /> ` graph,` <br /> ` s: number = 1): number` | gets the total MST cost of weighted graph by Prim algorithm
`mstKruskal(graph): number` | gets the total MST cost of weighted graph by Kruskal algorithm
`mstKruskal(graph, k): number` | gets the max space of k-clustering by Kruskal algorithm
`sccKosaraju(graph): []` | gets the top 10 large size strong connect component of directed graph, using Kosaraju algorithm
`topologicalSort(graph): []` | gets the topological visiting array of this directed graph
`undirectedConnected(graph): []` | gets an array indicating connectivity info of undirected graph. this undirected graph is connected iff `result.length == 1` __AND__ `result[0][1] == Graph.dfs(graph)`

[Back to top](#graph)