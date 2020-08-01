---
parent: Classes
title: biolink:EnvironmentalFeature
grand_parent: Browse Biolink Model
layout: default
---

# Type: EnvironmentalFeature




URI: [biolink:EnvironmentalFeature](https://w3id.org/biolink/vocab/EnvironmentalFeature)


---

![img](http://yuml.me/diagram/nofunky;dir:TB/class/[PlanetaryEntity],[PlanetaryEntity]%5E-[EnvironmentalFeature|id(i):string;name(i):label_type;category(i):category_type%20%2B])

---


## Parents

 *  is_a: [PlanetaryEntity](PlanetaryEntity.md) - Any entity or process that exists at the level of the whole planet

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