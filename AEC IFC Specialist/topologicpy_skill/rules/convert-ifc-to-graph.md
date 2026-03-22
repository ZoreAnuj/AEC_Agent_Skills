Title: Convert IFC to Topologic Graph

Overview:
- Use ifcopenshell to parse IFC, extract relevant topologies (IfcBuildingStorey, IfcSpace, IfcWall, IfcSlab).
- Convert extracted topologies or geometry to Topologic / topologicpy cell complexes and then use Graph.ByTopology to build a graph.

Minimal snippet:

```python
import ifcopenshell
import topologicpy
from topologicpy.Graph import Graph
# open IFC and extract topologies (example assumes cell_complex constructed)
model = ifcopenshell.open("building.ifc")
# build cell_complex from IFC entities (user-specific mapping)
cell_complex = ...
graph = Graph.ByTopology(cell_complex, direct=True, viaSharedTopologies=True, toExteriorTopologies=True, useInternalVertex=True, storeBREP=True, tolerance=1e-4)
```

Notes:
- Retain GlobalId and property sets by mapping IFC entity ids to graph node dictionaries.
- Defeature large geometry before conversion to improve performance.
- Use Graph.Topology to retrieve a cluster for visualization.
