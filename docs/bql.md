# Querying the graph: BQL, or the BadWolf Query language

BadWolf provides a high level declarative query and update language. BQL
(or BadWolf Query Language) is a declarative language losely modeled after
[SPARQL](https://en.wikipedia.org/wiki/SPARQL) to fit the temporal nature of
BadWolf graph data.

## BQL Grammar Organization

The BQL grammar is expressed as a LL1 and implemented using a recursively
descent parser. The grammar can be found in the
[grammar file](../bql/grammar/grammar.go).
The initial version of the grammar is available, as well as the lexical and
syntactical parser.

Semantic, planner, optimizer, and executer for BQL are currently work in
progress.

## Supported

BQL currently supports three statements:

* _Select_: Allows querying data form one or more graphs.
* _Insert_: Allows inserting data form one or more graphs.
* _Delete_: Allows deleting data form one or more graphs.