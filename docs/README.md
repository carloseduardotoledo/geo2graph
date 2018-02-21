
# geo2graph

The inital effort of this proposition will be using Esri ArcGIS Geodatabase as the GIS source of data and topological relations,  [ArcGIS API for Python](https://developers.arcgis.com/python/), Python, Cypher and Neo4j as the destination Graph Database.

Feature Classes will be extract, transformed, and load as Graph Nodes while spatial relations will be ETLed as Graphs Edges.

## Alpha Version - Proof of Concept
1. Read two Esri Geodatabase Feature Classes and build Cypher script to write features as Neo4j Nodes labeling feature with the Feature Class name;
1. Create contains inside buffer relations and write results as Neo4j Edges;
1. Delete Nodes without relations (Edges) from and to.
