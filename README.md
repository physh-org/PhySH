# [PhySH - Physics Subject Headings](https://physh.org/)

PhySH is provided in RDF largely using the entities and relationships defined by [SKOS](https://www.w3.org/2009/08/skos-reference/skos.html). We have added to the RDF vocabulary using a custom ontology with canonical URI  https://physh.org/rdf/2018/01/01/core# (prefix "physh_rdf" in what follows) - this defines the following classes:

- `physh_rdf:Discipline` as type for disciplines; these are also of type skos:ConceptScheme
- `physh_rdf:Facet` as type for facets; these are also of type skos:Concept
- `physh_rdf:Concept` skos:Concept's that are *not* facets.

and the following properties:

- `physh_rdf:contains` - facet contains this concept
- `physh_rdf:deprecated` - concept should no longer be used
- `physh_rdf:excludeFromIndexing` - concept should not be returned as a search result 
- `physh_rdf:hasConcept` - discipline has this concept
- `physh_rdf:inDiscipline` - concept is in a particular discipline
- `physh_rdf:inFacet` - concept is in a particular facet
- `physh_rdf:prefLabel` - like skos:prefLabel, but applies to concept schemes also
- `physh_rdf:usedByDiscipline` - facet is used by this discipline
- `physh_rdf:usesFacet` - discipline uses this facet

Note that `contains` and `inFacet` are inverses, as are `hasConcept` and `inDiscipline`, and `usedByDiscipline` and `usesFacet`; the PhySH RDF files include both sides of these relations. We also use the Dublin core terms vocabulary (http://purl.org/dc/terms/ - dcterms) to provide metadata for the concept schemes/disciplines.
