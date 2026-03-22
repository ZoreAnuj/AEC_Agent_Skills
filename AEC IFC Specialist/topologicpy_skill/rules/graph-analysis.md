Title: Graph analysis for building data

Overview:
- Common analyses: shortest path, adjacency matrix, MST, degree sequence, topological distance.

Examples:

```python
from topologicpy.Graph import Graph
# adjacency
adj_list = Graph.AdjacencyList(graph)
adj_matrix = Graph.AdjacencyMatrix(graph)
# shortest path
path = Graph.ShortestPath(graph, start_vertex, end_vertex)
# MST
mst = Graph.MinimumSpanningTree(graph)
# degree sequence
degrees = Graph.DegreeSequence(graph)
```

Notes:
- Convert node/edge attributes to numeric features for Graph ML frameworks.
- Use Graph.Topology to visualize nodes/edges with Plotly helpers.
