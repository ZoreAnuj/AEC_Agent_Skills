Title: Preparing Topologic graphs for Graph Machine Learning

Overview:
- Export adjacency matrix/list and node/edge features to DGL or PyG formats.

Example workflow:

```python
import numpy as np
from topologicpy.Graph import Graph
# nodes and edges
vertices = Graph.Vertices(graph)
edges = Graph.Edges(graph)
# build adjacency
adj = Graph.AdjacencyMatrix(graph)
# extract features from Topology dictionaries
features = [Topology.Dictionary(v) for v in vertices]
# convert to numpy arrays and feed to DGL/PyG
```

Notes:
- Ensure consistent node ordering when building adjacency and feature arrays.
- Normalize numeric attributes and encode categorical attributes.
- Store mapping between Topologic vertex ids and graph node indices to trace results back to the model.
