## SPARQL Shorthand

| Shorthand  | Full Form           | Usage Example                         |
|------------|---------------------|---------------------------------------|
| `a`        | `rdf:type`          | `?x a foaf:Person.` |
| `PREFIX`   | Namespace shortcut  | `PREFIX foaf: <http://xmlns.com/foaf/0.1/>` |
| `SELECT *` | Wildcard selection  | `SELECT * WHERE { ?s ?p ?o. }` |
| `BIND`     | Assign variable     | `BIND(STR(?name) AS ?stringName)` |
| `FILTER`   | Condition check     | `FILTER (?age > 18)` |
| `OPTIONAL` | Include if exists   | `OPTIONAL { ?person foaf:age ?age. }` |
| `UNION`    | Combine queries     | `{ ?x foaf:knows ?y } UNION { ?x foaf:colleague ?y }` |
| `VALUES`   | List-based filter   | `VALUES ?color { "Red" "Blue" "Green" }` |
| `SERVICE`  | Query external data | `SERVICE <https://query.wikidata.org/sparql> { ... }` |
| `CONSTRUCT`| Generate RDF triples| `CONSTRUCT { ?x foaf:knows ?y } WHERE { ... }` |

