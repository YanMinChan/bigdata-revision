﻿# Knowledge Representation
This is some notes I make from the slides and extra materials I found online

## Raw data to RDF
1. Protege
* We can manually define OWL classes and relationships, then import CSV data in protege

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
* RDF is able to define basic data model using triples ([subject][predicate][object])
* However, they couldn't add more advanced logic (i.e a child has 2 parents, a book must have at least one author, the parent of an elephant is also an elephant)

### Examples
* There are some example of RDF triples in RDF/XML syntax (.xml)and their respective Turtle syntax (.ttl) version
    * [rdf_xml-1](rdf_xml-1.xml) & [turtle-1](turtle-1.ttl)
    * [rdf_xml-2](rdf_xml-2.xml) & [turtle-2](turtle-2-standalone_uri.ttl)
    * [rdf_xml-3](rdf_xml-3.xml) & [turtle-3](turtle-3-blank_node.ttl)
    * [rdf_xml-4](rdf_xml-4.xml) & [turtle-4](turtle-4.ttl)
    * Note: The RDF/XML version is generated by ChatGPT and the Turtle version is translated by me (for better understanding of RDF structure).
* Some revision notes
    * Blank nodes (Turtle syntax) [[link](https://www.w3.org/TR/turtle/#BNodes)]

## Basic OWL(Web Ontology Language)
* Add rich reasoning to RDF. Organizes and enriches RDF data.
* Provides reasoaning support (i.e a child has 2 parents).

### Terminology
* TBox: the ontology (knowledge model) with concepts (class hierarchy) and relationships.
* ABox: the data instances (individuals) as per the ontology

### Ontology
* **Meta data**: Data describing the content and meaning of resources
    * ie: `<owl:imports>`
* **Terminologies**: Shared common vocabs
* **Ontologies**: Shared and common knowledge of a domain
* To easily create Ontology, use Protege

### Ontology Reasoning
* Consistency checking: ABox does not contradict TBox
* Concept satisfiability: Possibility of adding individuals to class
    * Can a class (ie. Course) have individuals?
* Classification: Create full inheritance hierarchy to answer questions
    * Does class A subsumes class B (ie. Is a student a person? If yes then does concept of person satisfy a student?)
* Realisation: Compute the direct type (class) of each individual
    * Individual X is a student

## Advanced OWL
