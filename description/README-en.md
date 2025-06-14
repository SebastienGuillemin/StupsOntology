# STUPS&copy; ontology

This repository contains an ontology describing the knowledge of French scientific experts used in illicit drug analysis. Note that the ontology is written in French (a translation will be uploaded in the future).

The last version of the ontology (*STUPS.ttl*) can be found at the root of the repository. Previous versions are available in the folder "/old".

## Ontology description
This ontology is made up of 19 concepts, 44 object properties and 40 data properties.
Note that elements of this ontology are in French, as it was planned to be used by the French scientific police.


| **Concept**            | **Description** |
|--------------------------|-----------------|
| **Echantillon**          | A drug sample belongs to a sealed evidence bag ("scellé"). A sample is identified by a sample number (a string), its drug type ('cannabis', 'cocaine', 'miscellaneous', or 'amphetamine and derivatives'), macroscopic characteristics, an external appearance, potentially an internal appearance, an active ingredient, and cutting agents. Experts may also provide comments on the sample. Additionally, a sample may be linked to other samples. In cases where chemical profiling is performed, each sample is associated with a chemical profile. |
| **Aspect**               | An aspect describes the internal or external appearance of a sample. |
| **Composant**            | A component of a sample is either an active ingredient or a cutting agent. A component is linked to a substance and optionally to a dosage (expressed as a mass percentage). |
| **Departement**          | A department is within a region and contains one or more cities. |
| **FormeChimique**       | A chemical form is associated with an active ingredient to describe its chemical nature. The chemical forms considered in the STUPS ontology are: Base, HCL, Base and HCL, Sulfate, Hydrochloride, Phosphate, or Undetermined. |
| **Pays**                 | A country contains one or more regions. |
| **Pic**                  | A peak in a chemical profile characterizes a chemical compound (molecule) present in the sample. Each peak is defined by a retention time and an area, corresponding to the quantity of the target compound in the sample. |
| **PrincipeActif**       | An active ingredient is the main substance in a sample. Every active ingredient has a chemical form. |
| **ProduitCoupage**      | A cutting agent is a substance that makes up part of a sample. |
| **ProfilChimique**      | A chemical profile is associated with a sample for the purpose of chemical profiling. A chemical profile represents a chromatogram made up of a set of peaks that indicate the presence of target chemical compounds. |
| **ProfilChimiqueCocaine**| A cocaine profile contains 18 peaks corresponding to residual solvents used during cocaine production. These are not always all present, as it depends on the production process. |
| **ProfilChimiqueHeroine**| A heroin profile contains 6 peaks corresponding to impurities that depend on the production (synthesis) process. They are always present but may vary in quantity. |
| **Region**               | A region contains one or more departments and is located within a country. |
| **Saisine**              | A *saisine* is a legal term used in procedural matters. It refers to the action taken by a requesting service when requesting the analysis of a drug seizure. The record (i.e. all related information) of a *saisine* of a presumed illicit product includes a capturing service, a requesting service, the city where the *saisine* was made, and the destination country of the product. This information may be complete or partial. Additionally, a *saisine* includes a set of sealed evidence bags (*scellés*). |
| **Scelle**               | *Scellés* (sealed evidence bags) are included in a *saisine*. Each *scellé* contains one or more samples of the substances to be identified and is identified by a unique number. A *scellé* is a court-ordered measure intended to preserve evidence for judicial use. It can also refer to the act of sealing with wax. |
| **Service**              | There are two types of services: requesting services and capturing services. All services are identified by a name. Additionally, a service is located in a city and may be associated with various administrative information (telephone number, etc.). |
| **ServiceCapteur**       | A capturing service is the entity that performs the drug seizure. |
| **ServiceRequerant**     | A requesting service is the entity that requests the analysis of a drug seizure (i.e. the originator of the *saisine*). |
| **Substance**            | The concept of substance here matches that used in chemistry. It is used to represent the substance linked to the components of a sample (active ingredient and cutting agent), as well as to the peaks in a chemical profile. A substance has a name. |
| **Ville**                | A city is located in a department. |


## Use this ontology
If you use this ontology (or a part of this ontology), please cite our work using as follows:\
Sébastien GUILLEMIN, Laurence DUJOURDY, Ludovic JOURNAUX, Ana ROXIN: STUPS&copy; Ontology, 2024, *Laboratoire d'Informatique de Bourgogne*, available online: https://github.com/SebastienGuillemin/StupsOntology.git.
