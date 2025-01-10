# Optimisation Bi-Objectif pour un Tramway Hybride LAC/Batterie

Introduction

Le transport ferroviaire joue un rôle clé dans la mobilité durable, mais il est confronté à des défis techniques, notamment dans la gestion efficace de l'énergie. Ce projet vise à modéliser et optimiser un système d'alimentation électrique hybride pour tramway combinant une ligne aérienne de contact (LAC) et une batterie embarquée. L'objectif est de réduire les chutes de tension aux bornes du train tout en minimisant les coûts liés à la batterie.

Ce travail s'inscrit dans une démarche d'optimisation multi-critères en utilisant des techniques avancées telles que Monte Carlo et l'algorithme génétique NSGA-2 pour identifier les solutions Pareto-optimales.

émarches Réalisées

1. Modélisation du Système

Le système étudié comprend :

Sous-stations : Générateurs de tension avec résistances internes, connectées au réseau public.

Ligne aérienne de contact (LAC) et rails : Modélisés avec des résistances linéiques.

Train : Charge mobile caractérisée par sa position, sa vitesse, et sa puissance mécanique (positive ou négative en fonction des phases de mouvement).

La simulation inclut :

Le déplacement du tramway entre deux sous-stations.

Le calcul des tensions, courants, et puissances dans chaque branche du réseau.
3. Algorithme Génétique NSGA-2

L'algorithme génétique NSGA-2 permet d’optimiser simultanément plusieurs objectifs avec un nombre réduit d’évaluations. Sa mise en œuvre comprend :

Initialisation : Création d’une population initiale de solutions potentielles.

Évaluation : Calcul des objectifs (capacité de la batterie et chute de tension maximale) pour chaque individu.

Sélection : Basée sur la dominance de Pareto pour conserver les meilleures solutions.

Croisement et mutation : Génération de nouvelles solutions en combinant et modifiant les solutions existantes.

Les résultats montrent que NSGA-2 converge rapidement vers un front de Pareto bien réparti, réduisant le besoin en calculs par rapport à Monte Carlo.
L’impact d’un système de batterie embarquée pour stocker l’énergie lors des freinages.

2. Méthode de Monte Carlo

La méthode Monte Carlo est utilisée pour explorer l’espace de solutions en générant un grand nombre de points dans l’espace des décisions. Cette approche brute permet de :

Évaluer les performances : Calculer les chutes de tension maximales et les capacités requises pour chaque solution.

Identifier les solutions Pareto-optimales : Mettre en évidence les compromis entre coût (capacité de la batterie) et robustesse (réduction des chutes de tension).
Bien que Monte Carlo soit efficace pour une exploration exhaustive, elle nécessite de nombreuses évaluations, ce qui justifie l’usage d’algorithmes plus sophistiqués.

But du Projet

L'objectif principal de ce projet est de concevoir un système d’alimentation hybride LAC/batterie pour tramway permettant de :

Réduire les chutes de tension aux bornes du train, garantissant ainsi une alimentation stable et conforme aux normes.

Minimiser les coûts associés à la batterie en optimisant sa capacité.

En combinant des outils de simulation et d’optimisation avancés, ce travail met en évidence les compromis nécessaires entre performance et coût dans la conception de systèmes ferroviaires.

Conclusion

Ce projet démontre l’importance des approches multi-critères pour résoudre des problématiques complexes dans le domaine ferroviaire. La méthode Monte Carlo fournit une vue d’ensemble des solutions possibles, tandis que NSGA-2 permet d’obtenir des solutions optimales avec une efficacité accrue.

Les résultats obtenus montrent que l’ajout d’un système de batterie embarquée permet de réduire significativement les chutes de tension et d’améliorer la robustesse du système d’alimentation, tout en maintenant des coûts raisonnables. Cette étude constitue une base solide pour des recherches futures sur le dimensionnement et le contrôle optimal des systèmes d’alimentation ferroviaires.

