# Ontologie STUPS&copy; (FR)

Ce dépôt contient une ontologie décrivant les connaissances des experts de la police scientifique en matière d'analyse des drogue. Notez que l'ontologie est écrite en français (une traduction sera mise en ligne dans le futur).

La dernière version de l'ontologie (*STUPS.ttl*) se trouve à la racine du dépôt. Les versions précédentes sont disponibles dans le dossier "/old".

## Description de l'ontology
Cette ontologie est constituée de 19 concepts, 45 propriétés d'objet et 44 propriété de données.

Une définition des différents concepts est données dans le tableau suivant.

| **Concept**            | **Description** |
|--------------------------|-----------------|
| **Echantillon**          | Un échantillon de stupéfiant appartient à un scellé. Un échantillon est caractérisé par un numéro d’échantillon (une chaîne de caractères), son type de drogue ('cannabis', 'cocaïne', 'divers' ou 'amphétamine et dérivés'), des caractéristiques macroscopiques, un aspect externe, potentiellement un aspect interne, un principe actif et des produits de coupage. Les experts peuvent aussi donner des commentaires sur l’échantillon. De plus, un échantillon peut être lié à d'autres échantillons. Dans le cas des stupéfiants sur lesquels une analyse de profilage chimique est réalisée, chaque échantillon est associé à un profil chimique. |
| **Aspect**               | Un aspect décrit l’aspect interne ou externe d’un échantillon. |
| **Composant**            | Un composant d'un échantillon est soit un principe actif soit un produit de coupage. Un composant est lié à une substance et éventuellement à un dosage (exprimé en pourcentage massique). |
| **Departement**          | Un département est dans une région et a une ou plusieurs villes. |
| **FormeChimique**       | Une forme chimique est associée à un principe actif pour décrire sa forme chimique. Les formes chimiques considérées dans l'ontologie STUPS sont : Base, HCL, Base et HCL, Sulfate, Chlorhydrate, Phosphate ou Indéterminée. |
| **Pays**                 | Un pays a une ou plusieurs régions. |
| **Pic**                  | Un pic d’un profil chimique caractérise un composé chimique (molécule) présent dans l’échantillon. Chaque pic est caractérisé par un temps de rétention et une aire, correspondant à la quantité du composé cible dans l’échantillon. |
| **PrincipeActif**       | Un principe actif est la principale substance d’un échantillon. Tout principe actif a une forme chimique. |
| **ProduitCoupage**      | Un produit de coupage est une substance composant un échantillon. |
| **ProfilChimique**      | Un profil chimique est associé à un échantillon dans le but de faire du profilage chimique. Un profil chimique représente un chromatogramme constitué d’un ensemble de pics permettant d’identifier la présence de composés chimiques cibles. |
| **ProfilChimiqueCocaine**| Un profil de cocaïne a 18 pics correspondant à des solvants résiduels ayant servi dans la fabrication de la cocaïne. Ils ne sont pas toujours tous présents, cela dépend du procédé de fabrication. |
| **ProfilChimiqueHeroine**| Un profil d'héroïne a 6 pics correspondant à des impuretés dépendant du procédé de fabrication (synthèse). Elles sont toujours présentes mais les quantités peuvent être différentes. |
| **Region**               | Une région a un ou plusieurs départements et est dans un pays. |
| **Saisine**              | Une saisine est un terme juridique utilisé en matière de procédure. Elle désigne l'action qu'accomplit un requérant lorsqu'il demande l'analyse d'une saisie de stupéfiant. La fiche (i.e. l’ensemble des informations) d’une saisine d’un produit supposé illicite contient un service capteur, un service requérant, la ville où la saisine a été faite et le pays de destination du produit. Ces renseignements peuvent être complets ou partiels. De plus, une saisie contient un ensemble de scellés. |
| **Scelle**               | Les scellés sont contenus dans une saisine. Chaque scellé contient un ou plusieurs échantillons des produits à identifier et est identifié par un numéro unique. Un scellé est une mesure ordonnée, afin de conserver les pièces à conviction à la disposition de la justice. Il peut désigner également le fait d'apposer un cachet de cire sur une pièce à conviction. |
| **Service**              | Il existe deux types de services : les services requérants et les services capteurs. Tous les services sont identifiés par un nom. De plus, un service est localisé dans une ville et peut être associé à un certain nombre d’informations administratives (numéro de téléphone, etc.). |
| **ServiceCapteur**       | Un service capteur est le service qui réalise la saisie de stupéfiant. |
| **ServiceRequerant**     | Un service requérant est le service qui requiert l’analyse d’une saisie de stupéfiants (i.e. celui à l’origine de la saisine). |
| **Substance**            | Le concept de substance est le même que celui de la chimie. Ici, il est utilisé pour représenter la substance à laquelle sont reliés les composants d’un échantillon (principe actif et produit de coupage) ainsi que les pics d’un profil chimique. Une substance a un nom. |
| **Ville**                | Une ville est dans un département. |



## Utiliser cette ontologie
Si vous utilisez cette ontologie (ou une partie de cette ontologie), veuillez citer notre travail comme suit :\
Sébastien GUILLEMIN, Laurence DUJOURDY, Ludovic JOURNAUX, Ana ROXIN: Ontologie STUPS&copy;, 2024, *Laboratoire d'Informatique de Bourgogne*, disponible en ligne: https://github.com/SebastienGuillemin/StupsOntology.git.