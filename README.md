# geo2graph

Geo2Graph is an initiative to transform geographic information systems data into graph databases, allowing the use of graph algebra and algorithms to analyze topological relations. 

The inital effort of this initiative will be using Esri ArcGIS Geodatabase as the GIS source of data and topological relations,  [ArcGIS API for Python](https://developers.arcgis.com/python/), [Python](https://www.python.org/), Cypher and [Neo4j](https://neo4j.com/) as the destination Graph Database.

Feature Classes will be extract, transformed, and load as Graph Nodes while spatial relations will be ETLed as Graphs Edges.

## Alpha Version
### Requirements
The first functinal version of geo2graph shoud: 
1. Read Esri Geodatabase Feature Classes and build Cypher script to writing features as Neo4j Nodes labeling feature with the Feature Class name;
1. Create topological relation (inside buffer) and write results as Neo4j Edges;
1. Delete Nodes without Edges.
