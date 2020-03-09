# RDF-RDFS-RDFa-OWL-TTL-XML
 Semantic web, linked datasets

## Good practises

### Principles of linked open data

* On the web
* Machine Readable
* Non-proprietary format
* RSF standards
* Linked RDF

Get an overview of the principles of Linked Data with ["Linked Data: Evolving the Web into a Global Data Space" by Tom Heath and Christian Bizer](http://linkeddatabook.com/editions/1.0/)

### Syntax

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

#### Reference biblio on good practices

[A pattern catalogue for modelling, publishing, and consuming Linked Data by Leigh Dodds and Ian Davis](https://patterns.dataincubator.org/book/)


## Resources for semantic web

### Find datasets and ontologies

[Visualize the Linked Open Data Cloud on lod-cloud.net](https://lod-cloud.net/)
[![License: CC BY 4.0](https://licensebuttons.net/l/by/4.0/80x15.png)](https://creativecommons.org/licenses/by/4.0/)  
View and search ontologies and datasets classified by topics.

### Enrich plain text

[Annotate text with DBpediaSpotlight](https://www.dbpedia-spotlight.org/demo/) (with API too)