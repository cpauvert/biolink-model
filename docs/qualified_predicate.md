---
parent: Edge Properties
title: biolink:qualified_predicate
grand_parent: Slots
layout: default
---

# Slot: qualified_predicate


Predicate to be used in an association when subject and object qualifiers are present and the full reading of the statement requires a qualification to the predicate in use in order to refine or  increase the specificity of the full statement reading.  This qualifier holds a relationship to be used instead of that  expressed by the primary predicate, in a ‘full statement’ reading of the association, where qualifier-based  semantics are included.  This is necessary only in cases where the primary predicate does not work in a  full statement reading.

URI: [biolink:qualified_predicate](https://w3id.org/biolink/vocab/qualified_predicate)

## Domain and Range

[Association](Association.md) ->  <sub>0..1</sub> [String](types/String.md)

## Parents

 *  is_a: [association slot](association_slot.md)

## Children


## Used by

 * [DeprecatedPredicateMapping](DeprecatedPredicateMapping.md)