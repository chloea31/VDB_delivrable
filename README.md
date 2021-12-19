# BIOGEOGRAPHIE MICROBIENNE DES SURFACES DES TOILETTES PUBLIQUES


## Table des matières
1. [Description](#descrp)
2. [Exigences](#exi)
3. [Utilisation](#utilisation)
4. [Auteur](#auteur)
5. [Références](#ref)


<a name="descrp"></a> 

## Description

L'objectif principal de l'étude consiste à tenter de comprendre et décrire la diversité microbienne dans les environnements intérieurs.
Une question générale que nous pourrions nous poser serait la suivante : Quelles sont les caractéristiques des différentes communautés bactériennes en terme d'abondance et de distribution dans les différents environnements?
Pour tenter de répondre à cette problématique, nous avons divisé le travail en 3 parties :
1. Quelles différences en terme d'abondance entre les différentes surfaces ?
2. Quelles différences entre les hommes et les femmes ?
3. Quelles corrélations pourrions-nous établir entre phylum, échantillons et surfaces ?

<a name="exi"></a> 

## Exigences

#### Installer miniconda3:

[Miniconda](https://docs.conda.io/en/latest/miniconda.html#linux-installers)

#### Installer krona:

[Krona](https://hpc.nih.gov/apps/kronatools.html)(https://github.com/marbl/Krona/wiki/Installing)

#### Créer l'environnement à partir du fichier my_env.yml : 
``` conda env create -f my_env.yml ```

#### Activer l'environnement env_vdb:
``` conda activate env_vdb ```

<a name="utilisation"></a> 

## Utilisation

#### Pour faire tourner le pipeline:
Cliquer sur ```Cell``` puis ```Run all```

#### Après exécution, le script produira les outputs suivants:
- un fichier nommé ```VDB16S_prepared.txt```, contenant les données préparées pour les analyses.
- plusieurs graphiques effectués avec Plotly, notamment:
    - des barplots, représentant les fréquences d'abondance des phylums sur chaque surface, ainsi que les fréquences d'abondance des surfaces pour chaque genre de bactérie. Grâce aux barplots, nous pouvons voir si certains phylums ne sont présents que sur certaines surfaces. Nous pouvons également voir les surfaces sur lesquelles il y a une grande diversité microbienne.
    - une treemap et un graph krona, représentant le genre de bactérie, le genre (homme ou femme), et la surface, ainsi que les proportions des genres de bactéries. La treemap permet de mettre en évidence les proportions des genres de bactérie et de les "ordonner". Le graph krona "cache" une partie de la complexité et présente un aspect interactif.
    - les graphiques en 3 dimensions pour l'ACP. Cette dernière permet de réduire les dimensions d'un jeu de données. Ici, nous avons considéré les genres de bactéries (diminution des dimensions du jeu de données) pour réduire le nombre de dimensions à 3 dimensions, avoir la possibilité de les afficher et potentiellement identifier des clusters.

<a name="authors"></a> 

## Auteur

Le projet a été développé par Chloé Aujoulat.

<a name="ref"></a> 

## Références
Flores, Gilberto E., Scott T. Bates, Dan Knights, Christian L. Lauber, Jesse Stombaugh, Rob Knight, et Noah Fierer. « Microbial Biogeography of Public Restroom Surfaces ». PLOS ONE 6, nᵒ 11 (23 novembre 2011): e28132. https://doi.org/10.1371/journal.pone.0028132.
