# Ontologie STUPS&copy; (FR)

Ce dépôt contient une ontologie décrivant les connaissances des experts de la police scientifique en matière d'analyse des drogue. Notez que l'ontologie est écrite en français (une traduction sera mise en ligne dans le futur).

La dernière version de l'ontologie (*STUPS.ttl*) se trouve à la racine du dépôt. Les versions précédentes sont disponibles dans le dossier "/old".

## Description de l'ontology
Cette ontologie est constituée de 20 concepts, 45 propriétés d'objet, 40 propriété de données et 95953 individus.

Une définition des différents concepts est données dans le tableau suivant.

|Concept|Definition|
|-------|----------|
|Aspect|Un aspect permet de d’écrire l’aspect interne ou l’aspect externe d’un échantillon.|
|Composant|Un composant est utilisé pour décrire ce qui compose un échantillon. Il en existe deux types : les principes actifs et les produits de coupages. Un composant est lié à une substance et éventuellement a un dosage (exprimé en pourcentage massique).|
|Departement|Un département est dans une région et a une ou plusieurs villes.|
|Echantillon|Un échantillon de drogue est extrait à partir d’un prélèvement d’un scellé. Un échantillon est caractérisé par un numéro d’échantillon et son type de drogue ('cannabis', 'cocaïne', 'divers' ou 'amphétamine et dérivés'). Un échantillon a des caractéristiques macroscopiques (aspect internes et externes, couleurs etc.), un principe actif et des produits de coupage. Les experts peuvent aussi donner des commentaires sur l’échantillon. De plus, un échantillon peut être regroupé avec d’autres échantillon dans un lot.|
|FormeChimique|Une forme chimique (Base, HCL, Base et HCL, Sulfate, Chlorhydrate, Phosphate ou Indéterminée) est associée à un principe actif pour décrire sa forme chimique.|
|Pays|Un pays a une ou plusieurs régions|
|Pic|Un pic d’un profil chimique caractérise un composé chimique (molécule) présent dans l’échantillon. Chaque pic est caractérisé par un temps de rétention et une aire, correspondant à la quantité du composé cible dans l’échantillon.|
|PrincipeActif|Un principe actif est la principale substance d’un échantillon. Tout principe actif a une forme chimique.|
|ProduitCoupage|Un produit de coupage est une substance composant un échantillon. Ce produit de coupage est en plus petite quantité que le principe actif.|
|ProfilChimique|Un profil chimique est associé à un échantillon dans le but de faire du profilage (i.e. rapprocher automatique des échantillons selon leur profil et leurs caractéristiques). Un profil chimique représente chromatogramme constitué d’un ensemble de pics  permettent d’identifier la présence ou composés chimiques cible.|
|ProfilChimiqueCocaine|Un profil de cocaïne a 18 pics, correspondant à des solvants résiduels ayant servi dans la fabrication de la cocaïne, sont recherchés. Ils ne sont pas toujours tous présents, cela dépend du procédé de fabrication   (extraction).|
|ProfilChimiqueHeroine|Pour l’héroïne, 6 pics correspondant à des impuretés   et dépendent du procédé de fabrication (synthèse). Elles sont toujours présentes mais les quantités peuvent être différentes.|
|Region|Une région a un ou plusieurs département est dans un un pays.|
|Saisine|La saisine est un terme juridique utilisé en matière de procédure. Elle désigne l'action qu'accomplit un requérant lorsqu'il demande l'analyse d'une saisie de drogue. La fiche (i.e. l’ensemble des informations) d’une saisine d’un produit supposé illicite contient un service capteur, un service requérant, la ville où la saisine a été faite et le pays de destination du produit. Ces renseignements peuvent être complets ou partiels. De plus, une saisie contient un ensemble de scellés|
|Scelle|Les scellés sont contenus dans une saisine. Chaque scellé contient un ou plusieurs échantillons des produits à identifier et est identifié par un numéro unique. Un scellé est une mesure ordonnée, afin de conserver les pièces à conviction à la disposition de la justice.  Il peut désigner également le fait d'apposer un cachet de cire sur une pièce à conviction.|
|Service|Il existe deux types de services : les services requérants et les services capteurs. Tous les services sont identifiés par un nom. De plus un service est localisé dans une ville et peut être associé à un certain nombre d’informations administratives (numéro de téléphone etc.).|
|ServiceCapteur|Un service capteur est le service qui réalise la saisie de drogue.|
|ServiceRequerant|Un service requérant est le service qui requiert l’analyse d’une saisie de drogue (i.e. celui à l’origine de la saisine).|
|Substance|Le concept de substance est le même que celui de la chimie. Ici, il est utilisé pour représenter la substance à laquelle sont reliés les composants d’un échantillon (Principe actif et Produit de coupage) ainsi que les pics d’un profil. Une substance à un nom.|
|Ville|Un ville est dans un département.|

## Requêtes SPARQL

Le dépôt contient aussi à la racine un fichier (*queries.rq*) contenant des requêtes SPARQL implémentant certaines règles d'analyse utilisée par la police scientifique.

## Utiliser cette ontologie
Si vous utilisez cette ontologie (ou une partie de cette ontologie), veuillez citer notre travail comme suit :\
Sébastien GUILLEMIN, Laurence DUJOURDY, Ludovic JOURNAUX, Ana ROXIN: Ontologie STUPS&copy;, 2024, *Laboratoire d'Informatique de Bourgogne*, disponible en ligne: https://github.com/SebastienGuillemin/StupsOntology.git.