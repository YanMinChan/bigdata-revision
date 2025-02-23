# Knowledge Representation
This is some notes I make from the slides

## RDF

### Schema vs. Instance
Think of schema as a form and instance as a filled out form.
1. Schema (blueprint)
* defines the structure of the data
* classes, properties, shared vocab
* i.e. for a book (class), it hasTitle (property)

2. Instance
* actual data that conforms to the schema
* represent specific object
* i.e. a particular book (Harry Potter)

## RDF Vocabularies

### SKOS (Simple Knowledge Organization System)
A standard vocabulary for organizing knowledge, specialised for thesauri, classification etc.

[SKOS Vocabularies](https://www.w3.org/2009/08/skos-reference/skos.html)

### Limitation
* RDF is able to define basic data model using triples (<subject><predicate><object>)
* RDFS (RDF Schema) adds basic structure, such as class and properties
* However, they couldn't add more advanced logic (i.e a child has 2 parents, a book must have at least one author, the parent of an elephant is also an elephant)

## OWL(Web Ontology Language)
* Add rich reasoning to RDF. Organizes and enriches RDF data.
