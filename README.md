# Projet RH - Analyse de l'Attrition et Leviers de Fidélisation
**Un enjeu clé de performance**

---

## TL;DR

Ce projet explore les dynamiques d’attrition à travers une analyse RH structurée en trois axes : profil des salariés, contexte organisationnel et dimensions subjectives.

Il met en évidence des configurations de risque et propose des leviers de fidélisation, dans un cadre strictement exploratoire et non causal.

Le constat clé est que l'attrition est un phénomène multifactoriel et progressif, résultant de l'interaction entre ces différentes dimensions.

L'approche RH doit ainsi s'inscrire dans une logique de prévention ciblée plutôt que dans des actions isolées.

---

## Résumé stratégique

### Problématique

> Quels sont les effets individuels et combinés des conditions de travail, des facteurs personnels et du niveau de satisfaction et d'implication sur l'attrition des salariés ?

### Approche analytique

Pour chaque axe, une analyse exploratoire descriptive a été menée afin de décrire la population, le contexte organisationnel et le ressenti des salariés.

Les variables ont ensuite été croisées avec l'attrition afin d'identifier des différences de comportement et des configurations à risque.

Une synthèse transversale a enfin permis de relier les axes et de mettre en évidence des dynamiques communes, dans un cadre strictement descriptif et non causal.

### Constats clés 

- L'attrition est un phénomène multifactoriel et progressif, et non un événement isolé.

- Les trajectoires de départ se construisent dans le temps, à travers l'accumulation de facteurs individuels, organisationnels et subjectifs.

- Les perceptions subjectives jouent un rôle intermédiaire cumulatif : elles traduisent l'accumulation de tensions plutôt qu'un déclencheur immédiat du départ.

- Certaines phases de parcours, notamment les premières années ou les périodes de transition, constituent des zones de vulnérabilité accrues.

### Leviers RH identifiés

- Sécuriser les phases de transition, notamment lors des premières années et des mobilités internes.

- Stabiliser l'environnement organisationnel à travers le management, la charge de travail et les politiques de rémunération.

- Agir sur les mécanismes intermédiaires d'attrition en renforçant la reconnaissance et l'engagement.

- Mettre en place une logique de prévention ciblée plutôt que des actions isolées.

### Limites 

Cette analyse est strictement descriptive : aucun lien de causalité n'est établi et l'absence de modélisation prédictive limite l'estimation de l'impact relatif des facteurs et du risque individuel.

Certaines dimensions structurantes ne sont pas mesurées, ce qui implique une lecture prudente des résultats.

Enfin, le jeu de données étant fictif et limité à un contexte spécifique à un instant donné, la généralisation des résultats reste restreinte.

### Outils

- Python (pandas, numpy)
- Matplotlib
- Seaborn
- Jupyter Notebook
- VS Code
  
---

## Liens des notebooks du projet

1. [Exploration initiale des données](notebooks/01_rh_exploration.ipynb)
2. [Définition des Axes selon les variables](notebooks/02_create_interim_tableaux.ipynb)
3. [Axe 1 – Conditions personnelles](notebooks/03_axe_1_conditions_personnelles.ipynb)
4. [Axe 2 – Conditions de travail](notebooks/04_axe_2_conditions_travail.ipynb)
5. [Axe 3 – Satisfaction et implication](notebooks/05_axe_3_satisfaction_implication.ipynb)
6. [Synthèse transversale et recommandations RH](notebooks/06_synthese_recommandations.ipynb)

---

# Analyse détaillée

## Contexte RH

La maîtrise de l'attrition constitue aujourd'hui un enjeu majeur pour les services RH : elle permet de limiter les coûts liés aux départs, de stabiliser les équipes et de mieux gérer la charge de travail.

La fidélisation des collaborateurs devient ainsi un levier clé : la capacité d'une entreprise à retenir ses talents conditionne directement sa performance opérationnelle, son engagement interne et sa compétitivité.

Disposer d'une analyse claire des facteurs d'attrition permet d'orienter les décisions RH, de prioriser les actions et de mettre en place des leviers de fidélisation efficaces.

---

## Objectif business

Analyser le dataset IBM HR Analytics Employee Attrition & Performance afin d’identifier les facteurs associés à l’attrition et d’orienter les décisions RH en matière de fidélisation.

---

## Problématique

Quels sont les effets individuels et combinés des conditions de travail, des facteurs personnels et du niveau de satisfaction et d'implication sur l'attrition des salariés ?

---

## Questions d'analyse

- **1. Conditions personnelles**  
Quel est l'impact des conditions de vie personnelles sur le départ des collaborateurs ?

- **2. Conditions de travail**  
Dans quelle mesure les conditions de travail influencent-elles l'attrition ?

- **3. Satisfaction et implication**  
Comment le niveau de satisfaction et d'implication contribue-t-ils à l'attrition ?  
Les conditions de travail et les facteurs personnels influencent-ils ces dimensions subjectives ?

---

## Données et approche analytique

L'analyse repose sur le jeu de données IBM HR Analytics Employee Attrition & Performance, un dataset fictif conçu par IBM, contenant 1 470 employés et plus de 30 variables RH.

Ce jeu de données contient des informations individuelles sur les employés, incluant :

- des caractéristiques personnelles (âge, genre, statut marital, etc.),
- des variables liées aux conditions de travail (poste, département, ancienneté, rémunération, environnement de travail, etc.),
- des indicateurs de satisfaction et d'implication,
- une variable cible indiquant le départ ou non de l'employé (**Attrition**).

Dans ce cadre exploratoire et descriptif, sans prétention causale, l'approche adoptée vise à identifier des relations entre variables.

L'analyse s'appuie principalement sur :
- des tableaux de proportions,
- des visualisations graphiques simples,
- des indicateurs de sur- et sous-exposition à l'attrition.

Certaines variables ont été transformées (tranches, regroupements, renommage) afin de faciliter l'interprétation RH.

---

## Comment naviguer dans le projet

Les notebooks sont conçus pour être lus dans l'ordre suivant :

1. `01_rh_exploration.ipynb` : exploration initiale du dataset
2. `02_create_interim_tableaux.ipynb` : structuration des variables par axes d'analyse
3. `03_...` à `05_...` : analyses par axe (préparation et analyse réalisées dans chaque notebook)
4. `06_...` : synthèse transversale et recommandations RH

Chaque notebook charge et enregistre les données via des chemins relatifs (`pathlib`), garantissant la reproductibilité du projet.

---

## Principaux enseignements

L'attrition ne résulte pas d'un facteur unique, mais de la combinaison :

- de phases de transition du parcours de vie (jeune âge),
- de situations professionnelles peu stabilisées (poste récent, faible ancienneté, relation managériale récente),
- de conditions organisationnelles spécifiques (notamment la rémunération),
- et de perceptions subjectives progressivement dégradées (satisfaction, engagement).

Cette lecture transversale met en évidence des trajectoires de départ construites dans le temps, plutôt qu'un événement ponctuel.

### Configurations de risque identifiées

- Jeunes salariés en début de parcours
- Salariés expérimentés en phase de transition
- Salariés commerciaux en forte mobilité

---

## Leviers RH identifiés

Les leviers identifiés se distinguent entre actions opérationnelles à impact court terme et leviers structurels inscrits dans une logique de transformation durable.

### Parcours

- **Renforcer l'onboarding managérial et le mentorat**
Sécuriser les premières phases du parcours collaborateur, identifiées comme périodes à risque accru d'attrition.

- **Politique d'intégration, de mentorat et de suivi des nouveaux salariés et des mobilités internes**
Sécuriser des dynamiques de parcours lors des premières années (professionnel, relationnel et culturel).
Améliorer l'expérience collaborateur et renforcer la cohésion et la culture d'entreprise.

### Management

- **Accompagnement managérial ciblé**
Stabiliser les relations manager-collaborateur, levier clé de satisfaction et d'engagement.

- **Modèle managérial et plan de formation**
Définir un cadre managérial commun (valeurs, posture, pratiques clés) et l'ancrer durablement par la formation.

### Engagement et conditions de travail

- **Reconnaissance non salariale**
Agir sur les mécanismes intermédiaires de l'attrition (satisfaction, engagement).
(retour managérial, reconnaissance symbolique, visibilité des contributions)

- **Vigilance sur les heures supplémentaires**
Limiter les effets cumulatifs dans des situations déjà fragilisées.

### Rémunération

- **Politique salariale ciblée sur les bas salaires**
Renforcer la rétention des populations les plus exposées au risque de départ, en particulier les salariés à bas salaire.

---

## Limites et perspectives

Cette analyse présente plusieurs limites inhérentes à son cadre méthodologique et aux données disponibles.


- **Limites liées à la méthode (EDA)**
Cette analyse ne permet pas d'établir de liens de causalité entre les facteurs étudiés et l'attrition.

De plus, l'absence de modélisation prédictive ne permet pas d'estimer l'impact relatif de chaque facteur ni de prédire le risque individuel de départ.

- **Limites liées aux variables**

L'analyse s'appuie sur un jeu de données contenant plusieurs variables auto-déclarées. Ces indicateurs peuvent être influencés par des biais de perception ou de déclaration.
Certaines dimensions importantes ne sont pas mesurées, telles que le climat social, la culture d'entreprise ou la qualité managériale réelle.
Certaines variables RH structurantes sont également absentes, notamment la distinction entre turnover volontaire et involontaire
ce qui implique une lecture prudente des résultats.

- **Limites liées au contexte**

Cette analyse repose sur un jeu de données fictif représentant une entreprise dans un contexte spécifique. Les résultats observés sont donc fortement dépendants de ce cadre.

L'approche adoptée offre une vision à un instant donné et ne permet pas d'analyser l'évolution des comportements ou des facteurs de risque dans le temps.

Enfin, ces éléments limitent la généralisation des résultats à d'autres organisations ou contextes sectoriels.

**Perspectives**

- **Modélisation logistique / Analyse multivariée ou segmentation**

Il serait pertinent de recourir à des méthodes de modélisation statistique, telles que la régression logistique, afin d'estimer l'effet combiné des facteurs identifiés sur l'attrition . Pour affiner la compréhension des profils et des configurations à risque, des analyses multivariées intégrant des interactions entre variables ou des segmentations seraient nécessaires.

- **Données longitudinales**

Cela permettrait de compléter l'analyse par une approche temporelle, en étudiant l'évolution des parcours, de la satisfaction et des comportements de départ dans le temps (limitées par la fictivité des données).

- **Suivi des leviers identifiés dans le temps (indicateurs de pilotage)**

Cela permettrait d'évaluer l'impact des actions mises en œuvre, d'ajuster les dispositifs d'accompagnement et de renforcer une démarche proactive de prévention de l'attrition.

---

## Conclusion - So what ?

Ce projet montre que l'attrition est un phénomène multifactoriel et progressif, résultant de l'interaction entre parcours, conditions de travail et ressenti des salariés.

Une approche RH efficace doit donc dépasser les actions isolées et s'inscrire dans une logique de prévention ciblée, en particulier lors des phases de transition professionnelles.

L'analyse exploratoire constitue ainsi une base solide pour orienter des actions RH plus fines et, à terme, des analyses prédictives.

---

## Définition of Done

- Données nettoyées et documentées  
- Analyse exploratoire descriptive complète  
- Identification des situations de sur/sous-exposition  
- Relations présentées sans interprétation causale  
- Visualisations claires  
- Recommandation RH exploitable
- Limites méthodologiques explicites  
