The library should follow the JVM cite library with methods implementing the following functionality.

Get component parts at top level:

get CTS namespace
get work component
get passage component
Get possible subordinate parts of work component:

get text group
get work
get version
get exemplar
Identify form of passage component:

is range (boolean)
has subref (boolean)
Get possible subordinate parts of passage component:

get node 1 (first node of range)
get subref 1 (subref on node 1)
get node 2 (second node of range)
get subref 2 (subref on node 2)
Convenience methods:

strip passage. Returns URN without passage component
reduce to work. Returns URN with work compoentn at notional work level.
reduce to version. Returns URN with work component at version level.