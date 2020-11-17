---
parent: Entities
title: biolink:Procedure
grand_parent: Classes
layout: default
---

# Class: Procedure


A series of actions conducted in a certain order or manner

URI: [biolink:Procedure](https://w3id.org/biolink/vocab/Procedure)

UMLSSG:PROC
{: .mapping-label }

UMLSSC:T058
{: .mapping-label }

UMLSST:hlca
{: .mapping-label }

UMLSSC:T059
{: .mapping-label }

UMLSST:lbpr
{: .mapping-label }

UMLSSC:T060
{: .mapping-label }

UMLSST:diap
{: .mapping-label }

UMLSSC:T061
{: .mapping-label }

UMLSST:topp
{: .mapping-label }

UMLSSC:T062
{: .mapping-label }

UMLSST:resa
{: .mapping-label }

UMLSSC:T063
{: .mapping-label }

UMLSST:mbrt
{: .mapping-label }

UMLSSC:T065
{: .mapping-label }

UMLSST:edac
{: .mapping-label }


---

![img](http://yuml.me/diagram/nofunky;dir:TB/class/[Occurrent]%5E-[Procedure%7Cid(i):string;name(i):label_type;category(i):category_type%20%2B],[Occurrent])

---


## Parents

 *  is_a: [Occurrent](Occurrent.md) - A processual entity

## Attributes


### Inherited from gene product:

 * [id](id.md)  <sub>REQ</sub>
    * Description: A unique identifier for a thing. Must be either a CURIE shorthand for a URI or a complete URI
    * range: [String](types/String.md)
    * in subsets: (translator_minimal)
 * [name](name.md)  <sub>REQ</sub>
    * Description: A human-readable name for a thing
    * range: [LabelType](types/LabelType.md)
    * in subsets: (translator_minimal)

### Inherited from named thing:

 * [category](category.md)  <sub>1..*</sub>
    * Description: Name of the high level ontology class in which this entity is categorized. Corresponds to the label for the biolink entity type class.
 * In a neo4j database this MAY correspond to the neo4j label tag.
 * In an RDF database it should be a biolink model class URI.
This field is multi-valued. It should include values for ancestors of the biolink class; for example, a protein such as Shh would have category values `bl:Protein`, `bl:GeneProduct`, `bl:MolecularEntity`, ...
In an RDF database, nodes will typically have an rdf:type triples. This can be to the most specific biolink class, or potentially to a class more specific than something in biolink. For example, a sequence feature `f` may have a rdf:type assertion to a SO class such as TF_binding_site, which is more specific than anything in biolink. Here we would have categories {bl:GenomicEntity, bl:MolecularEntity, bl:NamedThing}
    * range: [CategoryType](types/CategoryType.md)
    * in subsets: (translator_minimal)

## Other properties

|  |  |  |
| --- | --- | --- |
| **Mappings:** | | UMLSSG:PROC |
|  | | UMLSSC:T058 |
|  | | UMLSST:hlca |
|  | | UMLSSC:T059 |
|  | | UMLSST:lbpr |
|  | | UMLSSC:T060 |
|  | | UMLSST:diap |
|  | | UMLSSC:T061 |
|  | | UMLSST:topp |
|  | | UMLSSC:T062 |
|  | | UMLSST:resa |
|  | | UMLSSC:T063 |
|  | | UMLSST:mbrt |
|  | | UMLSSC:T065 |
|  | | UMLSST:edac |
