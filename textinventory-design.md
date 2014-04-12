# Text Inventory class #

Initial notes for behavior of a Text Inventory object.

## Constructor ##

Should accept XML serialization of TextInventory validating against CTS TextInventory schema.

## Metadata ##

- get cts namespace declarations
- get tiversion


## Basic document hierarchy ##

Identifying urns:

- get textgroups
- get works for textgroup
- get versions for work
- get exemplars for version

Labelling data:

- get textgroup name
- get work title
- get version label
- get exemplar label


## Data about documents ##

- determine if version is edition or translation
- get language for work
- get language for translation

## Citation data ##

- get all citation models
- for a citation model, find its depth
- for a citation model, get citation triplet at a given level
