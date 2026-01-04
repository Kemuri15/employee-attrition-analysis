# Projet RH – Analyse de l’Attrition et Leviers de Fidélisation
Un enjeu clé de performance

## Contexte RH

La maîtrise de l’attrition constitue aujourd’hui un enjeu majeur pour les services RH : elle permet de limiter les coûts liés aux départs, de stabiliser les équipes et de mieux gérer la charge de travail.
La fidélisation des collaborateurs devient ainsi un levier clé : la capacité d’une entreprise à retenir ses talents conditionne directement sa performance opérationnelle, son engagement interne et sa compétitivité.
Disposer d’une analyse claire des facteurs d’attrition permet d’orienter les décisions RH, de prioriser les actions et de mettre en place des leviers de fidélisation efficaces.

## Objectif business

Analyser le dataset IBM HR Analytics Employee Attrition & Performance afin d’identifier les facteurs associés à l’attrition et proposer des pistes d’action RH pour réduire les départs et augmenter la fidelisation comme levier de performance

Identifier les facteurs d’attrition à partir de l’analyse du dataset IBM HR Analytics afin d'orienter les décisions RH.
Proposer des recommandations permettant d’affiner la compréhension des leviers de fidélisation, enjeu essentiel de la performance sociale et globale de l’entreprise.

## Problématique

Quels sont les effets individuels et combinés des conditions de travail, des facteurs personnels et du niveau de satisfaction et d’implication sur l’attrition des salariés ?


## Questions d’analyse

**1. Conditions personnelles**  
Quel est l’impact des conditions de vie personnelles sur le départ des collaborateurs ?

**2. Conditions de travail**  
Dans quelle mesure les conditions de travail influencent-elles l’attrition ?

**3. Satisfaction et implication**  
Comment le niveau de satisfaction et d’implication contribue-t-il à l’attrition ?  
Les conditions de travail et les facteurs personnels influencent-ils le niveau de satisfaction et d’implication ?

## Données utilisées 

L’analyse repose sur le jeu de données **IBM HR Analytics Employee Attrition & Performance**, un dataset largement utilisé dans les projets d’analyse RH et de People Analytics,il s'agit d'un ensemble de données fictif créé par des data scientists d’IBM.

Ce jeu de données contient des informations individuelles sur les employés, incluant :
- des caractéristiques personnelles (âge, genre, situation familiale, niveau et domaine d’éducation, distance domicile–travail, mobilité professionnelle, etc.) ;
- des variables liées aux conditions de travail (poste, département, ancienneté, rémunération, environnement de travail, etc.) ;
- des indicateurs de satisfaction et d’implication ;
- une variable cible indiquant le départ ou non de l’employé (**Attrition**).

Le dataset comporte **1 470 employés** et **plus de 30 variables**, permettant d’explorer différents axes explicatifs de l’attrition.

Dans le cadre de ce projet, une sélection de variables pertinentes est effectuée et certaines d’entre elles sont transformées (création de tranches, regroupement de catégories, renommage des modalités) afin de faciliter l’analyse exploratoire et l’interprétation RH.


## Exploration des données (EDA)

Une analyse exploratoire des données (EDA) est menée afin de mieux comprendre la structure du jeu de données et la composition de la population étudiée.

L’EDA s’appuie sur :
- des tableaux de proportions ;
- des visualisations graphiques simples (principalement des barplots) ;
- une analyse descriptive progressive, sans interprétation prématurée.
- les résultats clés

L’exploration est organisée par **axes thématiques**, notamment :
- les caractéristiques personnelles des employés (âge, genre, situation familiale, niveau et domaine d’éducation, distance domicile–travail, mobilité professionnelle) ;
- les conditions de travail ;
- les indicateurs de satisfaction et d’implication.

Certaines variables numériques sont regroupées en catégories pertinentes d’un point de vue RH (tranches d’âge, distance domicile–travail, nombre d’entreprises précédemment travaillées) afin de rendre les analyses plus lisibles et exploitables.

L’analyse exploratoire est menée en quatres temps :
1. une analyse individuelle des variables pour décrire la population ;
2. des comparaisons simples entre ces variables et l’attrition afin d’identifier des différences de comportement entre les groupes.
3. une analyse des relations entre variables pour identifier certains patterns.
4. 
5. les résultats clés

Les résultats détaillés de cette exploration sont présentés et illustrés dans le notebook associé au projet.


## ✅ Definition of Done

- Un notebook propre et structuré
- Quelques visualisations pertinentes graphiques
- 1 section "So What ?" contenant trois conclusions et recommandations RH

## ▶️ Rejouer
Activer l'environnement puis ouvrir `notebooks/01_rh_exploration.ipynb`