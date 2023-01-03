# What is _Common Core_

Common Core (CC) is a collaborative effort between the involved parties to 
express  alignment approaches for their respective Knowledge Graphs.  It is not
intended this be the only or even the most capable approach to such alignment, 
it most surely will not be. 

Additionally, it should be noted that alignment can be both a technical and social 
thing.  Elements of this work will touch on both.  

In the above context then, CC is a mechanism to seek alignment between involved parties
to enable better use of the resources from the represented communities across
a wide surface of users.   

Technical alignment exist at many layers.


## SPARQL 1.1 Federates Search via Service?

However, while it is true this approach should allow SPARQL queries to be formed that 
can be federated via SERVICE, see [https://www.w3.org/TR/sparql11-federated-query/](https://www.w3.org/TR/sparql11-federated-query/)
for details, this is not the primary goal.  

Additional approaches would include being able to form SPARQL CONSTRUCT calls to form new 
triples or leveraging approach to subset or frame out data from a parent graph into 
a useful subset of triples for specific communities or use cases.  

Rather, the goal here is not to promote any given approach to use the graphs that validate 
to this common core shape, but simply ensure that whatever approach is developed works against the
shared graph shapes.

## Initial approach

* Generate SHACL shapes for the various SPARQL queries used by groups involved in this work
* Provide approaches for the application of these SHACL shapes in the triplestore or via tools like pySHACL
* Provide approaches for generating, sharing and reviewing the results of these validation processes



## Representation

JSON-LD and HTTP along with robots.txt, sitemaps and sitegraphs

Most of these above items can be seen as simple applications of web architecture approaches.


## Vocabulary

schema.org, geosparql, DCAT, other?   

It may be possible to leverage VOID, schema.org or Hydra to represent the vocabularies used.
However, since the SHACL shapes will validate against the use of vocabularies explicitly this may
really not be needed.   Rather it might be easy to "grep" the shapes for the range of vocabularies used. 

## Activity representation

PROV


## Query representation

SPARQL

## Validation 

SHACL

## Relationship to FAIR (or CARE?)

TBD
