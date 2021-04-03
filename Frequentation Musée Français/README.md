# Analyse de la fréquentation des muséee français entre 2013 et 2018

Lien vers le notebook <a href="https://www.kaggle.com/axelma/frequentation-musee-2013-2018" target="_blank">hebergé par Kaggle.com</a> ou visible sur <a href="./frequentation-musee-2013-2018.ipynb" target="_blank">Github<a>.

## Dataset
- <a href="https://www.data.gouv.fr/fr/datasets/frequentation-des-musees-de-france/" target="_blank">Fréquentation des musées de Fance (FMF)</a>, Philippe-Alexandre P., mis à jour le 8 février 2021, sous licence libre
- Création d'une carte de la France : <a href="https://www.data.gouv.fr/fr/datasets/contours-des-regions-francaises-sur-openstreetmap/" target="_blank">OpenStreetMap</a>, DGFiP, 2 janvier 2018, sous licence ODbL</a>

Travail préliminaire sur le dataset FMF :
Un premier travail de data cleaning a été effectué avec un script python.
Le dataset original présentait un petit coquille : une seule colonne stats (données les plus précieuse de ce dataset) était présente 
avec pour format du "semi-colon separeted file".
Le script remplace toutes les occurences de "payant:" par "", ";gratuit:" par "," et ";label-date:".
Lors de ces remplacement, on s'occupe donc de transformer les semi-colons en comma.
Enfin, le script remplace "stats" dans le header par "payant,gratuit,date".

## Table des matières de l'analyse

* [Description du Dataset](#description)
* [Data cleaning](#cleaning)
    - [Travail préliminaire](#travail-preliminaire)
    - [Informations inutiles](#informations-inutiles)
    - [Valeurs manquantes](#valeurs-manquantes)
    - [Ajout d'informations](#ajout-informations)
* [Analyse visuelle](#analyse-visuelle)
    - [Nombre de musee](#nombre-musee)
    - [Tendance générale](#tendance-generale)
    - [Nationalité des musées](#nationalite)
    - [Repartition des musées français](#repartition-musees-france)

[Toujours en cours de production]
