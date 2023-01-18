<img src="./docs/images/commoncorelogo.png" width="100">

# Common Core

The Common Core repo is a collaborative effort to describe and catalogue elements of a linked data
approach that facilitate FAIR data principles.   At present this is an effort between Ocean InfoHub,
POLDER and the NSF DeCODER projects.

The first product being explored is the idea of a catologue of patterns supporting interoperability.
This has the name, Pattern Asset Catalogue (PAC).

# Pattern Asset Catalogue (PAC)

## PAC is

A simple JSON-LD (ie RDF) profile to describe a data graph that:

* Provides metadata about a SHACL shape (itself an RDF graph)
* related queries (SPARQL)
* related services associated with the above
* related JSON-LD frames
* potential JSON schema files
* example data graphs
* connects the above to resolvable and established references of associated goals and patterns

The reason?

SHACL, frames and other elements express the structure of a graph.  Additionaly they
can connect these assets to aspects of FAIR principles or other related principes.  This
can aid in the discovery and description of the intended goals of these assets.


## PAC is NOT

This is NOT semantic integration.  It is not an ontology and does not provide any of the deep semantic
interoperability benefits that ontology and semantic integration based on ontologies can provide.

PAC is also NOT a new concept.  It is a influenced by. and attempts to borrow (steal) from, things such as
OGC STAC but also could be compared to things such as SQL global as view / local as view concepts.

Additionally, there are other projects such as WSMO  (https://www.w3.org/Submission/WSMO-primer/) that have
the potential to address these goals in a more enterprise approach.

## Worth a 1000 words

![shic.svg](./docs/images/overview.svg)

##  Why not just?

### Use SPARQL in SHACL

While SHACL AF does allow some use of SPARQL including SELECT and ASK, this is a not more complex as the non-RDF
SPARQL is mapped into the SHACL.  Also, complex SPARQL seems like it would be at least annoying to do in this approach.
For now the model of connecting the SPARQL as an external creative work or other type is proposed.


### Put it all in one graph file

Given that both schema.org and SHACL build on the common RDF data model it would be just as easy (and one can)
integrate all this information into one file.   Why have two files holding the information?  Part of this is just
the simplicity of the abstraction as this concept is judged for value.  Blending the two files together
in some ways burdens the proven SHACL work with the ShaC hypothesis.

### Just use SPARQL 1.1 Federates Search via Service?

However, while it is true this approach should allow SPARQL queries to be formed that 
can be federated via SERVICE, see [https://www.w3.org/TR/sparql11-federated-query/](https://www.w3.org/TR/sparql11-federated-query/)
for details, this is not the primary goal.  

Additional approaches would include being able to form SPARQL CONSTRUCT calls to form new 
triples or leveraging approach to subset or frame out data from a parent graph into 
a useful subset of triples for specific communities or use cases.  

Rather, the goal here is not to promote any given approach to use the graphs that validate 
to this common core shape, but simply ensure that whatever approach is developed works against the
shared graph shapes.

## PAC and principles like FAIR

What are the elements of FAIR we can encode into SHACL?  PIDs?  Vocabulary?
If not SHACL, VOID or some other way to describe?  schema.org?

Extend type Org to address FAIR?  Build off the RDA working group?

Or SDGs or essential variables


