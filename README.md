# RDF-RDFS-RDFa-OWL-TTL-XML
 Semantic web, linked datasets

# Resources for semantic web

## Good practises

### Principles of linked open data

* On the web
* Machine Readable
* Non-proprietary format
* RSF standards
* Linked RDF

Get an overview of the principles of Linked Data with ["Linked Data: Evolving the Web into a Global Data Space" by Tom Heath and Christian Bizer](http://linkeddatabook.com/editions/1.0/)

### Syntax

[RDF translator on appspot.com](http://rdf-translator.appspot.com/) from about any language to about any other. See also [easyrdf.org](http://www.easyrdf.org/converter)

[Visualize RDF](http://cltl.nl/visualrdf/) .

#### Download data of a certain negotiated format with `curl` command (Windows)

`-L` refers to the location  
`-H` refers to the header   
more info with curl --help

* rdf/xml `curl -o myFileName.xml -L -H "Accept: application/rdf+xml" myURI`
* json `curl -o myFileName.json -L -H "Accept: application/json" myURI`
* turtle `curl -o myFileName.ttl -L -H "Accept: text/turtle" myURI`
* html `curl -o myFileName.html -L -H "Accept: text/html" myURI`

#### Assign URI / Prefix URI

Use `#` separator for grouping, small coherent datasets, simple structures.  
Use `/` separator for big datasets, modularity, to be more precise.  
[Read more about cool URIs on W3]( https://www.w3.org/TR/cooluris/)

[Code/Decode a URL on meyerweb.com](https://meyerweb.com/eric/tools/dencoder/) 

[Find namespace associated with prefix on prefix.cc](http://prefix.cc/) [![License: CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-sa/4.0/)

Common prefixes  

| prefix | URI | comment |
| ------ | --- | ------- |
| owl | http://www.w3.org/2002/07/owl# | OWL vocabulary |
| rdfs | http://www.w3.org/2000/01/rdf-schema# | RDF schema vocabulary |
| rdf | http://www.w3.org/1999/02/22-rdf-syntax-ns# | RDF vocabulary |
| xsd | http://www.w3.org/2001/XMLSchema# | RDF compatible XSD types |
| foaf | http://xmlns.com/foaf/0.1/ | Friend Of A Friend social vocabulary |
| dc | http://purl.org/dc/elements/1.1/ | Dublin Core resources metadata vocabulary |
| db | http://dbpedia.org/ | DBpedia data |
| sh | http://www.w3.org/ns/shacl# | SHACL Shapes Constraints Language vocabulary|

#### Reference biblio on good practices

[A pattern catalogue for modelling, publishing, and consuming Linked Data by Leigh Dodds and Ian Davis](https://patterns.dataincubator.org/book/)

## Standards

[W3C recommendation on OWL](https://www.w3.org/TR/owl-features/)  
[W3C recommendation on RDFS](https://www.w3.org/TR/rdf-schema/)  
[W3C recommendation on RDF/turtle syntax](https://www.w3.org/TR/turtle/)  
[W3C recommendation on RDF/XML syntax](https://www.w3.org/TR/rdf-syntax-grammar/)  
[W3C RDF/XML validator](https://www.w3.org/RDF/Validator/rdfval) renders triples and graph  
[W3C recommendation on XML datatypes](https://www.w3.org/TR/xmlschema-2/)  
[W3C recommendation on SHACL syntax](https://www.w3.org/TR/shacl/)  
[W3C recommendation on SPARQL syntax](https://www.w3.org/TR/sparql11-query/)  

## Software

[Download standalone version of Corese from inria.fr](https://project.inria.fr/corese/download/) for SPARQL queries and SHACL checks  
[Download Protégé from stanford.edu](https://protege.stanford.edu/products.php#desktop-protege) for ontology edition   

### SPARQL endpoints

[DBpedia with Flint SPARQL editor](http://fr.dbpedia.org/sparqlEditor/)  
[DBpedia with Virtuoso](http://fr.dbpedia.org/sparql)  
[INSEE](http://rdf.insee.fr/sparql)

### Find datasets and ontologies

[Visualize the Linked Open Data Cloud on lod-cloud.net](https://lod-cloud.net/)
[![License: CC BY 4.0](https://licensebuttons.net/l/by/4.0/80x15.png)](https://creativecommons.org/licenses/by/4.0/)  
View and search ontologies and datasets classified by topics.

### Enrich plain text

[Annotate text with DBpediaSpotlight](https://www.dbpedia-spotlight.org/demo/) with API too