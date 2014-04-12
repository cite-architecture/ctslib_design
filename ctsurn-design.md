# CTS URN class

These notes describe behavior of a constructor and five categories of methods that a CTS URN library
in any language should implement.



## Constructor ##

Given a String value, should return a CTS URN object

## Get component parts at top level

Given a CTS URN object, methods should return String values:

- get CTS namespace
- get work component
- get passage component

## Get possible subordinate parts of work component

Given a CTS URN object, method should return a value from an enumerated set
of some type appropriate to the implementing language:

- get work level

Given a CTS URN object, methods should return String values:

- get text group
- get work
- get version
- get exemplar

## Identify form of passage component

Given a CTS URN object, methods should return boolean values:

- is range (boolean)
- has subref (boolean)

## Get possible subordinate parts of passage component
 
Given a CTS URN object, methods should return String values:

- get range beginning node
- get range end node
- get subref (subref on point node)
- get subref 1 (subref string on range beginning node)
- get subref 2 (subref on range end node)


Given a CTS URN object, methods should return integer values:

- get subref index (index on subreference on a point node)
- get subref index 1  (index on subreference on range beginning node)
- get subref index 2  (index on subreference on range end node)



## Convenience methods

Given a CTS URN object, methods should return String values:

- to string.  Should permit either return of raw string or of URI encoding of subreference strings and subreference index square brackets.
- strip passage. Returns URN without passage component
- reduce to work. Returns URN with work compoentn at notional work level.
- reduce to version. Returns URN with work component at version level.
