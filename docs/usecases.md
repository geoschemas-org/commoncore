# Use Cases

## About 
The start of some documentation related to use cases.  Whiel the examples imply only two participants (A and B) there obviously could be more ivolved parties. 

Reference the various [SPARQL UNION](https://en.wikibooks.org/wiki/SPARQL/UNION) approaches for inspiration on potential ways to connect A and B.

1. Simple UNION call based on the query criteria.  So the full results are a superset of site A and B
1. A query that uses some resources (likely a PID) from the results at site A to look for connecting results at site B.   
1. Sub-query, to populate associated properties from site B into the results from a qury at Site A (this is likely just the approach to doing the above case 2)