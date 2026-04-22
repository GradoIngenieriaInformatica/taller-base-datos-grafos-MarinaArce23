MATCH (p:Persona)-[:VIVE_EN]->(c1), (p)-[:AMIGO_DE]->(a)-[:VIVE_EN]->(c2)
WHERE c1 <> c2
RETURN DISTINCT p.nombre
