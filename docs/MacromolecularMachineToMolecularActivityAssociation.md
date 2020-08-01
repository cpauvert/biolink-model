---
parent: Classes
title: biolink:MacromolecularMachineToMolecularActivityAssociation
grand_parent: Browse Biolink Model
layout: default
---

# Type: MacromolecularMachineToMolecularActivityAssociation


A functional association between a macromolecular machine (gene, gene product or complex) and a molecular activity (as represented in the GO molecular function branch), where the entity carries out the activity, or contributes to its execution

URI: [biolink:MacromolecularMachineToMolecularActivityAssociation](https://w3id.org/biolink/vocab/MacromolecularMachineToMolecularActivityAssociation)


---

![img](http://yuml.me/diagram/nofunky;dir:TB/class/[Publication],[Provider],[OntologyClass],[MolecularActivity],[MolecularActivity]%3Cobject%201..1-%20[MacromolecularMachineToMolecularActivityAssociation|relation(i):uriorcurie;id(i):string;negated(i):boolean%20%3F],[FunctionalAssociation]%5E-[MacromolecularMachineToMolecularActivityAssociation],[MacromolecularMachine],[FunctionalAssociation])

---


## Parents

 *  is_a: [FunctionalAssociation](FunctionalAssociation.md) - An association between a macromolecular machine (gene, gene product or complex of gene products) and either a molecular activity, a biological process or a cellular location in which a function is executed

## Referenced by class


## Attributes


### Own

 * [macromolecular machine to molecular activity association➞object](macromolecular_machine_to_molecular_activity_association_object.md)  <sub>REQ</sub>
    * range: [MolecularActivity](MolecularActivity.md)

### Inherited from association:

 * [subject](subject.md)  <sub>REQ</sub>
    * Description: connects an association to the subject of the association. For example, in a gene-to-phenotype association, the gene is subject and phenotype is object.
    * range: [NamedThing](NamedThing.md)
 * [relation](relation.md)  <sub>REQ</sub>
    * Description: The relation which describes an association between a subject and an object in a more granular manner. Usually this is a term from Relation Ontology, but it can be any edge CURIE.
    * range: [Uriorcurie](types/Uriorcurie.md)
 * [object](object.md)  <sub>REQ</sub>
    * Description: connects an association to the object of the association. For example, in a gene-to-phenotype association, the gene is subject and phenotype is object.
    * range: [NamedThing](NamedThing.md)
 * [association➞id](association_id.md)  <sub>REQ</sub>
    * Description: A unique identifier for an association
    * range: [String](types/String.md)
    * in subsets: (translator_minimal)
 * [negated](negated.md)  <sub>OPT</sub>
    * Description: if set to true, then the association is negated i.e. is not true
    * range: [Boolean](types/Boolean.md)
 * [association type](association_type.md)  <sub>OPT</sub>
    * Description: connects an association to the type of association (e.g. gene to phenotype)
    * range: [OntologyClass](OntologyClass.md)
 * [qualifiers](qualifiers.md)  <sub>0..*</sub>
    * Description: connects an association to qualifiers that modify or qualify the meaning of that association
    * range: [OntologyClass](OntologyClass.md)
 * [publications](publications.md)  <sub>0..*</sub>
    * Description: connects an association to publications supporting the association
    * range: [Publication](Publication.md)
 * [provided by](provided_by.md)  <sub>0..*</sub>
    * Description: connects an association to the agent (person, organization or group) that provided it
    * range: [Provider](Provider.md)

### Inherited from functional association:

 * [functional association➞subject](functional_association_subject.md)  <sub>REQ</sub>
    * range: [MacromolecularMachine](MacromolecularMachine.md)
 * [functional association➞object](functional_association_object.md)  <sub>REQ</sub>
    * range: [GeneOntologyClass](GeneOntologyClass.md)

### Domain for slot:

 * [macromolecular machine to molecular activity association➞object](macromolecular_machine_to_molecular_activity_association_object.md)  <sub>REQ</sub>
    * range: [MolecularActivity](MolecularActivity.md)