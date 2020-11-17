---
parent: Associations
title: biolink:DiseaseOrPhenotypicFeatureAssociationToThingAssociation
grand_parent: Classes
layout: default
---

# Class: DiseaseOrPhenotypicFeatureAssociationToThingAssociation




URI: [biolink:DiseaseOrPhenotypicFeatureAssociationToThingAssociation](https://w3id.org/biolink/vocab/DiseaseOrPhenotypicFeatureAssociationToThingAssociation)


---

![img](http://yuml.me/diagram/nofunky;dir:TB/class/[Publication],[OntologyClass],[NamedThing],[DiseaseOrPhenotypicFeature]%3Csubject%201..1-%20[DiseaseOrPhenotypicFeatureAssociationToThingAssociation%7Cid(i):string;predicate(i):predicate_type;relation(i):uriorcurie;negated(i):boolean%20%3F],[DiseaseOrPhenotypicFeatureAssociationToThingAssociation]%5E-[DiseaseOrPhenotypicFeatureAssociationToLocationAssociation],[Association]%5E-[DiseaseOrPhenotypicFeatureAssociationToThingAssociation],[DiseaseOrPhenotypicFeatureAssociationToLocationAssociation],[DiseaseOrPhenotypicFeature],[Association],[Agent])

---


## Parents

 *  is_a: [Association](Association.md) - A typed association between two entities, supported by evidence

## Children

 * [DiseaseOrPhenotypicFeatureAssociationToLocationAssociation](DiseaseOrPhenotypicFeatureAssociationToLocationAssociation.md) - An association between either a disease or a phenotypic feature and an anatomical entity, where the disease/feature manifests in that site.

## Referenced by class


## Attributes


### Own

 * [disease or phenotypic feature association to thing association➞subject](disease_or_phenotypic_feature_association_to_thing_association_subject.md)  <sub>REQ</sub>
    * Description: disease or phenotype
    * range: [DiseaseOrPhenotypicFeature](DiseaseOrPhenotypicFeature.md)
    * Example:    
    * Example:    

### Inherited from association:

 * [association➞id](association_id.md)  <sub>REQ</sub>
    * Description: A unique identifier for an association
    * range: [String](types/String.md)
    * in subsets: (translator_minimal)
 * [association type](association_type.md)  <sub>OPT</sub>
    * Description: connects an association to the type of association (e.g. gene to phenotype)
    * range: [OntologyClass](OntologyClass.md)
 * [subject](subject.md)  <sub>REQ</sub>
    * Description: connects an association to the subject of the association. For example, in a gene-to-phenotype association, the gene is subject and phenotype is object.
    * range: [NamedThing](NamedThing.md)
 * [predicate](predicate.md)  <sub>REQ</sub>
    * Description: A high-level grouping for the relationship type. AKA minimal predicate. This is analogous to category for nodes.
    * range: [PredicateType](types/PredicateType.md)
 * [object](object.md)  <sub>REQ</sub>
    * Description: connects an association to the object of the association. For example, in a gene-to-phenotype association, the gene is subject and phenotype is object.
    * range: [NamedThing](NamedThing.md)
 * [relation](relation.md)  <sub>REQ</sub>
    * Description: The relation which describes an association between a subject and an object in a more granular manner. Usually this is a term from Relation Ontology, but it can be any edge CURIE.
    * range: [Uriorcurie](types/Uriorcurie.md)
 * [negated](negated.md)  <sub>OPT</sub>
    * Description: if set to true, then the association is negated i.e. is not true
    * range: [Boolean](types/Boolean.md)
 * [qualifiers](qualifiers.md)  <sub>0..*</sub>
    * Description: connects an association to qualifiers that modify or qualify the meaning of that association
    * range: [OntologyClass](OntologyClass.md)
 * [publications](publications.md)  <sub>0..*</sub>
    * Description: connects an association to publications supporting the association
    * range: [Publication](Publication.md)
 * [provided by](provided_by.md)  <sub>0..*</sub>
    * Description: connects an association to the agent (person, organization or group) that provided it
    * range: [Agent](Agent.md)

### Domain for slot:

 * [disease or phenotypic feature association to thing association➞subject](disease_or_phenotypic_feature_association_to_thing_association_subject.md)  <sub>REQ</sub>
    * Description: disease or phenotype
    * range: [DiseaseOrPhenotypicFeature](DiseaseOrPhenotypicFeature.md)
    * Example:    
    * Example:    