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

* Generals

| prefix | URI | comment |
| ------ | --- | ------- |
| owl | http://www.w3.org/2002/07/owl# | Web Ontology Language |
| rdfs | http://www.w3.org/2000/01/rdf-schema# | Resource Description Framework Schema |
| rdf | http://www.w3.org/1999/02/22-rdf-syntax-ns# | Resource Description Framework |
| rdfa | http://www.w3.org/ns/rdfa# | Resource Description Framework in Attributes |
| sh | http://www.w3.org/ns/shacl# | SHACL Shapes Constraints Language vocabulary |
| void | http://rdfs.org/ns/void# | Vocabulary of Interlinked Datasets |
| dcat | https://www.w3.org/ns/dcat# | Data CATalog vocabulary |

* Specialized

| prefix | URI | comment |
| ------ | --- | ------- |
| xsd | http://www.w3.org/2001/XMLSchema# | RDF compatible XSD types |
| foaf | http://xmlns.com/foaf/0.1/ | Friend Of A Friend social vocabulary |
| rel | http://purl.org/vocab/relationship/ | Relationship, extension of FOAF |
| skos | http://www.w3.org/2004/02/skos/core# | SKOS knowledge vocabulary |
| skosxl | http://www.w3.org/2008/05/skos-xl# | SKOS eXtenstion for Labels |
| dct (dcterms) | http://purl.org/dc/terms | Dublin Core Metadata Initiative : Metadata Terms |
| dc | http://purl.org/dc/elements/1.1/ | DCMI : Metadata Elements |
| dctype | http://purl.org/dc/dcmitype/ | DCMI Type vocabulary |
| prov | https://www.w3.org/ns/prov# | Provenance vocabulary |
| qb | http://purl.org/linked-data/cube# | Data Cube vocabulary |
| cc | http://creativecommons.org/ns# | Creative Common licenses |
| sawsdl | http://www.w3.org/ns/sawsdl# | Semantic Annotation for Web Services Description Language |
| ma | http://www.w3.org/ns/ma-ont# | Ontology for media resources |

* Datasets

| prefix | URI | comment |
| ------ | --- | ------- |
| db | http://dbpedia.org/ | DBpedia data |

#### Reference biblio on good practices

[A pattern catalogue for modelling, publishing, and consuming Linked Data by Leigh Dodds and Ian Davis](https://patterns.dataincubator.org/book/)

## Some Standards

[W3C recommendation on OWL](https://www.w3.org/TR/owl-features/)  
[W3C recommendation on RDFS](https://www.w3.org/TR/rdf-schema/)  
[W3C recommendation on RDF/turtle syntax](https://www.w3.org/TR/turtle/)  
[W3C recommendation on RDF/XML syntax](https://www.w3.org/TR/rdf-syntax-grammar/)  
[W3C recommendation on RDFa syntax](https://www.w3.org/TR/rdfa-core/) to embed RDF in html  
[Schema.org vocabulary](https://schema.org/) for structured data on the internet  
[W3C recommendation on XML datatypes](https://www.w3.org/TR/xmlschema-2/)  
[W3C recommendation on SHACL syntax](https://www.w3.org/TR/shacl/)  
[W3C recommendation on SPARQL syntax](https://www.w3.org/TR/sparql11-query/)  
[W3C recommendation on Data Cube vocabulary](https://www.w3.org/TR/vocab-data-cube/) for multi-dimensional data  
[W3C recommendation on Provenance Data Model PROV-DM](https://www.w3.org/TR/prov-dm/)  
[W3C recommendation on Provenance Ontology](https://www.w3.org/TR/prov-o/) that expressed PROV-DM with OWL2  
[W3C recommendation on Semantic Annotations for Web Services Description Language and XML Schema SAWDSDL](https://www.w3.org/TR/sawsdl/) that is an extension of WSDL  
[W3C recommendation on Ontology for Media Resources](https://www.w3.org/TR/mediaont-10/)

## Famous schemas

[SKOS Simple Knowledge Organization System homepage](https://www.w3.org/2004/02/skos/) has 4 classes and 28 properties in OWL  
[SKOS-XL SKOS eXtension for Labels homepage](https://www.w3.org/TR/skos-reference/skos-xl.html) to transform labels into resources  
[Dublin Core Metadata Initiative](https://www.dublincore.org/) to describe documents has 22 classes and 55 properties. Note that DC Elements is a subset of DC Terms. DC Type is a different vocabulary containing types of things that can be described using DC terms.  
[Creative Commons homepage](https://creativecommons.org/) to describe rights associated to a resource, has 6 main classes, 12 secondary classes and 11 properties  
[Friend Of A Friend specifications](http://xmlns.com/foaf/spec/) for social networkd, has 13 classes and 62 properties  
[Relationship is an extension of FOAF](https://vocab.org/relationship/) to describe relations between persons  
[Vocabulary of Interlinked Datasets](http://vocab.deri.ie/void) to describe datasets and linksets  
[Data Catalog Vocabulary recommendation](https://www.w3.org/TR/vocab-dcat-2/) to describe any dataset, not only rdf

## Software

[W3C RDF/XML validator](https://www.w3.org/RDF/Validator/rdfval) renders triples and graph from RDF/XML  
[Download standalone version of Corese from inria.fr](https://project.inria.fr/corese/download/) for SPARQL queries and SHACL checks  
[Download Protégé from stanford.edu](https://protege.stanford.edu/products.php#desktop-protege) for ontology edition   
[Get simple RDFa samples on rdfa.info](https://rdfa.info/play/)  
[W3C RDFa distiller and parser](https://www.w3.org/2007/08/pyRdfa/) to get triples from html  
[Map a given vocabulary](http://www.visualdataweb.de/webvowl/#foaf) or append `IRI = ...`

### SPARQL endpoints

[DBpedia with Flint SPARQL editor](http://fr.dbpedia.org/sparqlEditor/)  
[DBpedia with Virtuoso](http://fr.dbpedia.org/sparql)  
[INSEE](http://rdf.insee.fr/sparql)

### Find datasets and ontologies

[Visualize the Linked Open Data Cloud on lod-cloud.net](https://lod-cloud.net/) [![License: CC BY 4.0](https://licensebuttons.net/l/by/4.0/80x15.png)](https://creativecommons.org/licenses/by/4.0/) View and search ontologies and datasets classified by topics.  
[Visualize Linked Open Vocabularies LOV](https://lov.linkeddata.es/dataset/lov/)


### Enrich plain text

[Annotate text with DBpediaSpotlight](https://www.dbpedia-spotlight.org/demo/) with API too
