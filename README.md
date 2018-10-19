# XStandoff
XStandoff uses the XML notation together with a formal model ranging from multi-rooted trees up to GODDAGs (general ordered-descendant directed acyclic graph) and supports discontinuous elements, multiple parenthood and differentiation between dominance and containment.

# Origin
The XStandoff format (formerly known as Sekimo Generic Format, SGF) is an XML-based (meta) markup language developed during the Sekimo project at Bielefeld University. It allows for the storage and analysis of multi-dimensional (and possibly overlapping) annotations.
The X in XStandoff stands both for eXtended and eXtensible, since the format is an extension to the classic standoff approach and is modularly designed. XStandoff is based on the formal model of a multi-rooted tree (i.e. a set of trees span over the same primary data) – at least if one restricts oneself to not using discontinuous segments, in that case the formal model tends to be an rGODDAG – and is capable of using tree- and graph-based annotation models.

# Ranges
XStandoff (like other standoff formats) uses the character positions of the primary data to depict the positions where annotation elements occur, cf. the following listing:
```
  T  h  e     s  u  n     s  h  i  n  e  s     b  r  i  g  h  t  e  r  .

00|01|02|03|04|05|06|07|08|09|10|11|12|13|14|15|16|17|18|19|20|21|22|23|24
```
The character 'T' ranges from position 0 to 1, the character 'h' from 1 to 2, and so on. This information is used during the constructing of an XStandoff instance.
In contrast to other serialization formats for multi-dimensional and possible overlapping markup XStandoff tries to conserve as much of the former annotation format as possible.
