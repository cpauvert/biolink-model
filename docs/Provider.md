---
parent: Classes
title: biolink:Provider
grand_parent: Browse Biolink Model
layout: default
---

# Type: Provider


person, group, organization or project that provides a piece of information

URI: [biolink:Provider](https://w3id.org/biolink/vocab/Provider)

UMLSSG:ORGA
{: .mapping-label }

UMLSSC:T092
{: .mapping-label }

UMLSST:orgt
{: .mapping-label }

UMLSSC:T093
{: .mapping-label }

UMLSST:hcro
{: .mapping-label }

UMLSSC:T094
{: .mapping-label }

UMLSST:pros
{: .mapping-label }

UMLSSC:T095
{: .mapping-label }

UMLSST:shro
{: .mapping-label }


---

![img](http://yuml.me/diagram/nofunky;dir:TB/class/[Association]-%20provided%20by%200..*%3E[Provider|id(i):string;name(i):label_type;category(i):category_type%20%2B],[AdministrativeEntity]%5E-[Provider],[Association],[AdministrativeEntity])

---


## Parents

 *  is_a: [AdministrativeEntity](AdministrativeEntity.md)

## Referenced by class

 *  **[Association](Association.md)** *[provided by](provided_by.md)*  <sub>0..*</sub>  **[Provider](Provider.md)**

## Attributes


### Inherited from named thing:

 * [id](id.md)  <sub>REQ</sub>
    * Description: A unique identifier for a thing. Must be either a CURIE shorthand for a URI or a complete URI
    * range: [String](types/String.md)
    * in subsets: (translator_minimal)
 * [name](name.md)  <sub>REQ</sub>
    * Description: A human-readable name for a thing
    * range: [LabelType](types/LabelType.md)
    * in subsets: (translator_minimal)
 * [category](category.md)  <sub>1..*</sub>
    * Description: Name of the high level ontology class in which this entity is categorized. Corresponds to the label for the biolink entity type class. In a neo4j database this MAY correspond to the neo4j label tag
    * range: [CategoryType](types/CategoryType.md)
    * in subsets: (translator_minimal)

## Other properties

|  |  |  |
| --- | --- | --- |
| **Aliases:** | | agent |
|  | | group |
| **Mappings:** | | UMLSSG:ORGA |
|  | | UMLSSC:T092 |
|  | | UMLSST:orgt |
|  | | UMLSSC:T093 |
|  | | UMLSST:hcro |
|  | | UMLSSC:T094 |
|  | | UMLSST:pros |
|  | | UMLSSC:T095 |
|  | | UMLSST:shro |
