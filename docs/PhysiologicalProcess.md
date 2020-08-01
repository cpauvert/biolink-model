---
parent: Classes
title: biolink:PhysiologicalProcess
grand_parent: Browse Biolink Model
layout: default
---

# Type: PhysiologicalProcess




URI: [biolink:PhysiologicalProcess](https://w3id.org/biolink/vocab/PhysiologicalProcess)

UMLSSG:PHYS
{: .mapping-label }

UMLSSC:T032
{: .mapping-label }

UMLSST:orga
{: .mapping-label }

UMLSSC:T039
{: .mapping-label }

UMLSST:phsf
{: .mapping-label }

UMLSSC:T040
{: .mapping-label }

UMLSST:orgf
{: .mapping-label }

UMLSSC:T041
{: .mapping-label }

UMLSST:menp
{: .mapping-label }

UMLSSC:T042
{: .mapping-label }

UMLSST:ortf
{: .mapping-label }

UMLSSC:T043
{: .mapping-label }

UMLSST:celf
{: .mapping-label }

UMLSSC:T045
{: .mapping-label }

UMLSST:genf
{: .mapping-label }

UMLSSC:T201
{: .mapping-label }

UMLSST:clna
{: .mapping-label }


---

![img](http://yuml.me/diagram/nofunky;dir:TB/class/[BiologicalProcess]%5E-[PhysiologicalProcess|id(i):string;name(i):label_type;category(i):category_type%20%2B],[NamedThing],[BiologicalProcess])

---


## Identifier prefixes

 * GO
 * REACT

## Parents

 *  is_a: [BiologicalProcess](BiologicalProcess.md) - One or more causally connected executions of molecular functions

## Attributes


### Inherited from biological process or activity:

 * [enabled by](enabled_by.md)  <sub>0..*</sub>
    * Description: holds between a process and a physical entity, where the physical entity executes the process
    * range: [NamedThing](NamedThing.md)
    * in subsets: (translator_minimal)

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
| **Aliases:** | | physiology |
| **Mappings:** | | UMLSSG:PHYS |
|  | | UMLSSC:T032 |
|  | | UMLSST:orga |
|  | | UMLSSC:T039 |
|  | | UMLSST:phsf |
|  | | UMLSSC:T040 |
|  | | UMLSST:orgf |
|  | | UMLSSC:T041 |
|  | | UMLSST:menp |
|  | | UMLSSC:T042 |
|  | | UMLSST:ortf |
|  | | UMLSSC:T043 |
|  | | UMLSST:celf |
|  | | UMLSSC:T045 |
|  | | UMLSST:genf |
|  | | UMLSSC:T201 |
|  | | UMLSST:clna |
