# md-adapter

The MagicDraw (Cameo System Modeler) adapter framework for OML

This framework consists of two major parts:

* Profile Generator
The profile generator converts a set of OML vocabularies into a SysML profile that can be installed in Magicdraw enabling the modeler to use the source vocabulary concepts and relations in a UML model to create models with precise semantics.
The input vocabulary is given in two parts: the source vocabulary and an associated embedding vocabulary that establishes the relationship between each element of the source vocabulary and a target SysML element it will become a stereotype for.

* Export Adapter
The export adapter will transform SysML/UML models that apply profiles generated using the profile generator into OML. The exported OML models can be subsequently transformed to OWL and given to a reasoner to verify the consistency of the instance model with the vocabulary. The OWL data can also be stored in a graph database to make it accessible to queries.

These elements are not yet implemented in openCAESAR. The legacy verions are available in the legacy repo. The legacy versions use a legacy version of the OML language (OML-1).

* [profile generator](https://github.com/JPL-IMCE/profileGenerator)
* [md adapter]()
* [legacy vocabularies](https://github.com/JPL-IMCE/gov.nasa.jpl.imce.ontologies.public)
