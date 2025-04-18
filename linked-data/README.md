# Intro
## Web of Documents
* Identifiers: URLs
* Protocol: HTTP
* Encoding: HTML
* Links: `<a href='...'>`

## Web of Data
* Identifiers: IRIs (Internationalised Resource Identifier), used as names of graph nodes in RDF space. (ie. Bob, Heriot-Watt, 包子)
* Protocol: HTTP
* Encoding: RDF
* Links: Data reuse from internal or external using RDF (The 5 star linked open data [[source](https://5stardata.info/en/)])

### A Table of 5 star linked data

| Star   | Characteristic                                  | Format  |
|--------|-------------------------------------------------|---------|
| 1 star | Available on the internet under an open license | None    |
| 2 star | Available as a structured data                  | Tabular |
| 3 star | Available in a non-proprietary open format      | CSV     |
| 4 star | Available with URIs                             | URIs    |
| 5 star | Linking data to other data to provide context   | RDF     |

Linked Closed Data: If the Linked Data Principles is applied within an enterprise, no open license is needed.

### The 5Vs of Big Data

| Characteristic | Description                                            |
|----------------|--------------------------------------------------------|
| Volume         | The size of the data                                   |
| Velocity       | The speed of which data is generated                   |
| Variety        | The variety of data source                             |
| Veracity       | The quality of data (clean, dirty with noise)          |
| Value          | The insights the data generates (best selling product) |

## Semantic Web
* Linked web of data, using machine readable data such as RDF and OWL.
### Semantic Web Challenge
* Making data machines understandable
    * Requires disambiguation of terms
        * Paris_Hilton a foaf:Person .
        * Paris_Hilton a schema:Hotel .
* Machines infer knowledge
    * i.e. Knows Paris_Hilton refer to the Hotel in some context
### Semantic Web Stack of Technologies
[Figure](https://www.researchgate.net/figure/The-Semantic-Web-stack-The-dotted-area-includes-the-technologies-used-in-the-Web-of-Data_fig1_259646272)

We will cover
* Namespaces (IRIs)
* RDF
* OWL
* Logic (OWL Reasoning)


## Knowledge Graph
* Knowledge base (university course and students etc) structured as a graph
* Enables user to search for things and get relevant information to the query

### Knowledge Graph Construction
* Identify the entities/nodes (ie. Book, Author)
* Identify the relationships/edges (ie. writtenBy)