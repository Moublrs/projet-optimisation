# Optimisation Bi-Objectif pour un Tramway Hybride LAC/Batterie

Description:

Ce projet vise à modéliser, analyser et optimiser les performances d’un tramway à alimentation hybride combinant une ligne aérienne de contact (LAC) et une batterie embarquée. L’objectif principal est de résoudre un problème d’optimisation bi-objectif en minimisant :

Le coût de la batterie, proportionnel à sa capacité.

La chute de tension maximale (∆V_max) au cours du trajet.

Les méthodes principales employées sont :

Une approche Monte Carlo pour explorer l'espace de recherche.

L’algorithme génétique NSGA-2 pour trouver un front de Pareto optimisé.

Fonctionnalités:

Modélisation Physique

Calcul du déplacement, de la vitesse, et de l’accélération du tramway.

Estimation des puissances mécanique et électrique requises.

Analyse des courants et tensions dans les sous-stations.

Simulation:

Comparaison des performances avec et sans batterie.

Gestion de l’énergie entre la batterie, la LAC et les sous-stations.

Optimisation:

Monte Carlo : échantillonnage brut pour explorer l'espace des solutions.

NSGA-2 : génération des fronts de Pareto optimisés pour identifier les meilleurs compromis entre objectifs.

Visualisations

Déplacement et Vitesse du Tramway

Déplacement :


Vitesse :


Analyse des Puissances

Puissance consommée par le tramway :


Puissance fournie ou absorbée par la batterie :


Tensions et Courants

Tension aux bornes du tramway (avec et sans batterie) :


Courants dans le circuit :

Installation

Clonez le dépôt :
git clone <URL_DU_DEPOT>
cd <NOM_DU_DEPOT>

Installez les dépendances requises :
pip install numpy matplotlib deap

Utilisation:

Exécutez le script principal pour générer les simulations et visualisations :

python main.py

Les résultats incluent :

Simulation des dynamiques du tramway.

Comparaison des performances avec et sans batterie.

Graphiques montrant les évolutions des courants, tensions, et puissances.

Fronts de Pareto optimisés pour le coût de la batterie et ∆V_max.
