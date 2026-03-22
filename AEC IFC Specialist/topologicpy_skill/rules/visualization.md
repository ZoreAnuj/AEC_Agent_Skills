Title: Visualizing Topologic graphs

Overview:
- Use Graph.Topology to get a Topologic cluster then Plotly helpers to create 3D plots.

Example:

```python
from topologicpy.Graph import Graph
from topologicpy.Plotly import Plotly
cluster = Graph.Topology(graph)
data = Plotly.DataByTopology(cluster)
fig = Plotly.FigureByData(data)
fig.show()
```

Notes:
- Use defeaturing and encoded meshing to simplify geometry for visualization.
- Export to Speckle or save as BREP/OBJ for downstream viewers.
