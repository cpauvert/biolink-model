---
parent: Entities
title: biolink:Pathway
grand_parent: Classes
layout: default
---

# Class: Pathway




URI: [biolink:Pathway](https://w3id.org/biolink/vocab/Pathway)

GO:0007165
{: .mapping-label }

SIO:010526
{: .mapping-label }

PW:0000001
{: .mapping-label }

WIKIDATA:Q4915012
{: .mapping-label }


---

![img](http://yuml.me/diagram/nofunky;dir:TB/class/[PhysicalEntity],[ChemicalToPathwayAssociation]-%20object%201..1%3E[Pathway%7Cid(i):string;name(i):label_type;category(i):category_type%20%2B],[BiologicalProcess]%5E-[Pathway],[NamedThing],[ChemicalToPathwayAssociation],[BiologicalProcess])

---


## Identifier prefixes

 * GO
 * REACT
 * KEGG
 * SMPDB
 * PHARMGKB.PATHWAYS
 * WIKIPATHWAYS

## Parents

 *  is_a: [BiologicalProcess](BiologicalProcess.md) - One or more causally connected executions of molecular functions

## Referenced by class

 *  **[ChemicalToPathwayAssociation](ChemicalToPathwayAssociation.md)** *[chemical to pathway association➞object](chemical_to_pathway_association_object.md)*  <sub>REQ</sub>  **[Pathway](Pathway.md)**

## Attributes


### Inherited from biological process or activity:

 * [enabled by](enabled_by.md)  <sub>0..*</sub>
    * Description: holds between a process and a physical entity, where the physical entity executes the process
    * range: [PhysicalEntity](PhysicalEntity.md)
    * in subsets: (translator_minimal)

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
| **Mappings:** | | GO:0007165 |
|  | | SIO:010526 |
|  | | PW:0000001 |
|  | | WIKIDATA:Q4915012 |
