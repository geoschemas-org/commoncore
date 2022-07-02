<img src="./docs/images/commoncorelogo.png" width="100">

# Common Core

## About

A repository to explore developing guidance and validation around common graph shapes
to facilitate federated use of implementing Knowledge Graphs.

## SPARQL 1.1 Federates Search via Service?

So, while it is true this approach should allow SPARQL queries to be formed that 
can be federated via SERVICE, see [https://www.w3.org/TR/sparql11-federated-query/](https://www.w3.org/TR/sparql11-federated-query/)
for details, this is not the primary goal.  

Additional approaches would include being able to form SPARQL CONSTRUCT calls to form new 
triples or leveraging approach to subset or frame out data from a parent graph into 
a useful subset of triples for specific communities or use cases.  

The goal here is not to promote any given approach to use the graphs that validate 
to this common core shape, but rather simply ensure that whatever approach is developed and used
can be operating against know graph shapes.

## Initial approach

The SHACL shape will be formed by simple inspection of the various SPARQL queries and looking at the 
required and optional elements.  Since the primary sources for the various groups are using structured
data on the web we can leverage some approaches to sampling the resources from identified providers
and checking them against the SHACL shapes.  Whether we can programatically check the SPARQL queries 
with the SHACL shapes is unknown at this time.  


