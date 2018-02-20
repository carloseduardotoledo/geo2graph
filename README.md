# geo2graph

Geo To Graph is an initiative to transform geographic information systems data into graph databases, allowing the use of graph algebra and algorithms to analyze topological relations.

The initiative effort of this proposition will be using Esri ArcGIS Geodatabase as the GIS source of data and topological relations, ArcPy, Python, Cypher and Neo4j as the destination Graph Database.

Feature Classes will be extract, transformed, and load as Graph Nodes while spatial relations will be ETLed as Graphs Edges.

## Alpha Version - Proof of Concept
1. Read two Esri Geodatabase Feature Classes and build Cypher script to write features as Neo4j Nodes labeling feature with the Feature Class name;
1. Create contains inside buffer relations and write results as Neo4j Edges;
1. Delete Nodes without relations (Edges) from and to.
