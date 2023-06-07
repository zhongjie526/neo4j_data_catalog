# Data Catalog Knowledge Graph Analytics by Neo4j

```
from neo4j import GraphDatabase
from graphdatascience import GraphDataScience

# Configure Neo4j connection settings
neo4j_url = "neo4j+ssc://34.126.85.60:7687"
neo4j_user = "neo4j"
neo4j_password = "neo4j123"
neo4j_db = "neo4j"

# Create a Neo4j driver and GDS driver
driver = GraphDatabase.driver(neo4j_url, auth=(neo4j_user, neo4j_password),database=neo4j_db)
gds = GraphDataScience(neo4j_url,auth=(neo4j_user,neo4j_password),database=neo4j_db)

print(f"GDS Version: {gds.version()}")
```

GDS Version: 2.3.3