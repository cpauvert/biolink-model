---
parent: Classes
title: biolink:ClinicalTrial
grand_parent: Browse Biolink Model
layout: default
---

# Type: ClinicalTrial




URI: [biolink:ClinicalTrial](https://w3id.org/biolink/vocab/ClinicalTrial)


---

![img](http://yuml.me/diagram/nofunky;dir:TB/class/[ClinicalEntity]%5E-[ClinicalTrial|id(i):string;name(i):label_type;category(i):category_type%20%2B],[ClinicalEntity])

---


## Parents

 *  is_a: [ClinicalEntity](ClinicalEntity.md) - Any entity or process that exists in the clinical domain and outside the biological realm. Diseases are placed under biological entities

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