---
parent: Entities
title: biolink:PhenotypicFeature
grand_parent: Classes
layout: default
---

# Class: PhenotypicFeature




URI: [biolink:PhenotypicFeature](https://w3id.org/biolink/vocab/PhenotypicFeature)

UPHENO:0001001
{: .mapping-label }

SIO:010056
{: .mapping-label }

WIKIDATA:Q169872
{: .mapping-label }


---

![img](http://yuml.me/diagram/nofunky;dir:TB/class/[EntityToPhenotypicFeatureAssociation]-%20object%201..1%3E[PhenotypicFeature%7Cid(i):string;name(i):label_type;category(i):category_type%20%2B],[DiseaseOrPhenotypicFeature]%5E-[PhenotypicFeature],[OrganismTaxon],[EntityToPhenotypicFeatureAssociation],[DiseaseOrPhenotypicFeature],[BiologicalEntity])

---


## Identifier prefixes

 * HP
 * EFO
 * NCIT
 * UMLS
 * MEDDRA
 * MP
 * ZP
 * UPHENO
 * APO
 * FBcv
 * WBPhenotype
 * SNOMEDCT
 * MESH

## Parents

 *  is_a: [DiseaseOrPhenotypicFeature](DiseaseOrPhenotypicFeature.md) - Either one of a disease or an individual phenotypic feature. Some knowledge resources such as Monarch treat these as distinct, others such as MESH conflate.

## Referenced by class

 *  **[EntityToPhenotypicFeatureAssociation](EntityToPhenotypicFeatureAssociation.md)** *[entity to phenotypic feature association➞object](entity_to_phenotypic_feature_association_object.md)*  <sub>REQ</sub>  **[PhenotypicFeature](PhenotypicFeature.md)**
 *  **[BiologicalEntity](BiologicalEntity.md)** *[has phenotype](has_phenotype.md)*  <sub>0..*</sub>  **[PhenotypicFeature](PhenotypicFeature.md)**

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

### Inherited from thing with taxon:

 * [in taxon](in_taxon.md)  <sub>0..*</sub>
    * Description: connects a thing to a class representing a taxon
    * range: [OrganismTaxon](OrganismTaxon.md)
    * in subsets: (translator_minimal)

## Other properties

|  |  |  |
| --- | --- | --- |
| **Aliases:** | | sign |
|  | | symptom |
|  | | phenotype |
|  | | trait |
|  | | endophenotype |
| **Mappings:** | | UPHENO:0001001 |
|  | | SIO:010056 |
|  | | WIKIDATA:Q169872 |
