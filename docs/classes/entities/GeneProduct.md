---
parent: Entities
title: biolink:GeneProduct
grand_parent: Classes
layout: default
---

# Class: GeneProduct


The functional molecular product of a single gene. Gene products are either proteins or functional RNA molecules

URI: [biolink:GeneProduct](https://w3id.org/biolink/vocab/GeneProduct)

WIKIDATA:Q424689
{: .mapping-label }


---

![img](http://yuml.me/diagram/nofunky;dir:TB/class/[Transcript],[Protein],[OrganismTaxon],[GeneToGeneProductRelationship],[GeneProductIsoform],[GeneToGeneProductRelationship]-%20object%201..1%3E[GeneProduct%7Cname:label_type;description:narrative_text%20%3F;synonym:label_type%20%2A;xref:iri_type%20%2A;has_biological_sequence(i):biological_sequence%20%3F;id(i):string;category(i):category_type%20%2B],[GeneProduct]%5E-[Transcript],[GeneProduct]%5E-[Protein],[GeneProduct]%5E-[GeneProductIsoform],[GeneProduct]%5E-[RNAProduct],[GeneOrGeneProduct]%5E-[GeneProduct],[GeneOrGeneProduct],[Gene],[RNAProduct])

---


## Identifier prefixes

 * UniProtKB
 * gtpo
 * PR

## Parents

 *  is_a: [GeneOrGeneProduct](GeneOrGeneProduct.md) - a union of genes or gene products. Frequently an identifier for one will be used as proxy for another

## Children

 * [RNAProduct](RNAProduct.md)
 * [GeneProductIsoform](GeneProductIsoform.md) - This is an abstract class that can be mixed in with different kinds of gene products to indicate that the gene product is intended to represent a specific isoform rather than a canonical or reference or generic product. The designation of canonical or reference may be arbitrary, or it may represent the superclass of all isoforms.
 * [Protein](Protein.md) - A gene product that is composed of a chain of amino acid sequences and is produced by ribosome-mediated translation of mRNA
 * [Transcript](Transcript.md) - An RNA synthesized on a DNA or RNA template by an RNA polymerase

## Referenced by class

 *  **[GeneToGeneProductRelationship](GeneToGeneProductRelationship.md)** *[gene to gene product relationship➞object](gene_to_gene_product_relationship_object.md)*  <sub>REQ</sub>  **[GeneProduct](GeneProduct.md)**
 *  **[Gene](Gene.md)** *[has gene product](has_gene_product.md)*  <sub>0..*</sub>  **[GeneProduct](GeneProduct.md)**

## Attributes


### Own

 * [id](id.md)  <sub>REQ</sub>
    * Description: A unique identifier for a thing. Must be either a CURIE shorthand for a URI or a complete URI
    * range: [String](types/String.md)
    * in subsets: (translator_minimal)
 * [name](name.md)  <sub>REQ</sub>
    * Description: A human-readable name for a thing
    * range: [LabelType](types/LabelType.md)
    * in subsets: (translator_minimal)

### Inherited from genomic entity:

 * [has biological sequence](has_biological_sequence.md)  <sub>OPT</sub>
    * Description: connects a genomic feature to its sequence
    * range: [BiologicalSequence](types/BiologicalSequence.md)

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
| **Mappings:** | | WIKIDATA:Q424689 |
