# p6-Algorithm-Tarjan

A perl6 implementation of Tarjan's algorithm for finding strongly connected components in a directed graph. 

More information can be found at wikipedia.org/wiki/Tarjan's_strongly_connected_components_algorithm

```
use Algorithm::Tarjan;

my Algorithm::Tarjan $a .= new();

my %h;
# code to fill %h node->[successor nodes]

$a.init(%h);
say 'There are ' ~ $a.find-cycles() ~ ' cycle(s) in the input graph';
```
If there is a need for the sets of strongly connected components, they can be retrieved from $a.strongly-connected (an array of node names).

