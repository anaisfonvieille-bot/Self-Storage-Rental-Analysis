# 📦 Analyse de la location de box de stockage

🌐 **Langue :** [English](README.md) | Français

![Python](https://img.shields.io/badge/Python-Analyse%20de%20données-3776AB?logo=python&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-Tableau%20de%20bord-F2C811?logo=powerbi&logoColor=black)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Modèles%20prédictifs-2E8B57)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![Données](https://img.shields.io/badge/Données-Anonymisées-0078D4)
![Statut](https://img.shields.io/badge/Statut-En%20cours-orange)

## 📌 Présentation du projet

Ce projet a été réalisé pour une entreprise de location de box de stockage exploitant quatre centres.

L’entreprise disposait de données contractuelles réparties dans plusieurs fichiers, mais ne bénéficiait pas d’une solution d’analyse centralisée. Elle possédait également très peu d’informations permettant de définir de véritables profils clients.

L’objectif était de transformer les données contractuelles disponibles en informations utiles à la prise de décision, de construire un tableau de bord de pilotage avec Power BI et d’explorer des modèles prédictifs permettant d’identifier les contrats présentant un risque plus élevé de départ anticipé ou d’annulation.

> Les modèles facilitent la priorisation et la prise de décision. Ils ne remplacent pas l’analyse humaine.

## 🎯 Problématique de l’entreprise

L’entreprise souhaitait :

- Centraliser et nettoyer les données contractuelles provenant de plusieurs sources.
- Suivre son activité à l’aide de Power BI, qui n’était pas encore exploité.
- Identifier les types de contrats les plus susceptibles de se terminer après 4, 6 ou 12 mois.
- Analyser les profils contractuels les plus associés aux annulations avant la date de début du contrat.
- Prioriser les actions commerciales et de fidélisation.
- Déterminer quelles nouvelles données clients devraient être collectées à l’avenir.

## ✅ Objectifs du projet

| Objectif | Valeur pour l’entreprise |
|---|---|
| Regrouper les fichiers disponibles | Créer un jeu de données analytique unique et fiable |
| Améliorer la qualité des données | Produire des indicateurs cohérents et réutilisables |
| Construire un tableau de bord Power BI | Faciliter le suivi opérationnel de l’activité |
| Prédire les départs anticipés | Identifier les contrats nécessitant une attention particulière |
| Analyser les annulations | Mieux comprendre les profils contractuels récurrents |
| Recommander de nouvelles données à collecter | Améliorer les futures analyses et les modèles prédictifs |

## 🗂️ Périmètre des données

L’analyse repose sur des données contractuelles et opérationnelles anonymisées provenant de quatre centres de location de box.

Les données initiales étaient réparties dans huit fichiers. Elles ont été regroupées au sein d’un jeu de données analytique unique.

Les livrables publics ne contiennent ni données brutes de l’entreprise, ni noms d’employés, ni noms réels des centres, ni identifiants de contrats.

### Informations disponibles

- Statut et dates des contrats
- Caractéristiques des espaces de stockage
- Mode de paiement et périodicité
- Variables financières et fiscales des contrats
- Remises et variables contractuelles
- Informations anonymisées sur les centres

### Limites actuelles

L’entreprise ne collecte pas encore suffisamment d’informations permettant de définir précisément les profils clients.

Des variables telles que la tranche d’âge, la catégorie socioprofessionnelle, le canal d’acquisition, le motif de location, la satisfaction, le motif d’annulation ou le motif de départ n’étaient pas disponibles.

Par conséquent :

- Les modèles reposent principalement sur les caractéristiques contractuelles.
- Les relations observées ne doivent pas être interprétées comme des liens de causalité.
- Les prédictions servent à prioriser les actions et non à automatiser les décisions.
- Le taux d’occupation, la marge, la rentabilité nette et les délais réels de déménagement ne faisaient pas partie du périmètre disponible.

## 🛠️ Technologies utilisées

- **Python** — préparation des données, contrôles qualité et modélisation
- **Pandas / NumPy** — manipulation des données
- **Matplotlib / Seaborn** — visualisation exploratoire
- **Scikit-learn** — modélisation prédictive et évaluation
- **Jupyter Notebook** — documentation reproductible de l’analyse
- **Power BI** — tableau de bord opérationnel et décisionnel
- **Canva** — présentation métier et recommandations

## 🔄 Méthodologie

1. Regroupement des huit fichiers sources
2. Contrôle de la structure et de la qualité des données
3. Traitement des doublons, valeurs manquantes, dates, montants et pourcentages
4. Analyse exploratoire des contrats et des annulations
5. Construction des variables cibles pour les départs à 4, 6 et 12 mois
6. Prévention des fuites de données
7. Comparaison de la régression logistique, de l’arbre de décision et de la forêt aléatoire
8. Évaluation avec le ROC-AUC, le score F1, la précision, le rappel et les matrices de confusion
9. Interprétation à l’aide de l’importance par permutation et des taux observés par sous-groupe
10. Traduction des résultats en recommandations opérationnelles

## 🤖 Analyse prédictive

Deux analyses prédictives complémentaires ont été réalisées.

### Départ anticipé des contrats

Les modèles estiment quels contrats présentent des caractéristiques associées à un départ dans un délai de :

- 4 mois
- 6 mois
- 12 mois

La régression logistique, l’arbre de décision et la forêt aléatoire ont été comparés.

Les performances ont été évaluées à l’aide de plusieurs indicateurs complémentaires plutôt qu’avec la seule exactitude globale.

### Annulation avant le début du contrat

Un modèle distinct analyse les profils contractuels associés aux annulations réalisées avant la date de début prévue du contrat.

Ses performances prédictives sont considérées comme modérées. Il doit donc être utilisé comme une aide à la priorisation et non comme un outil de décision automatique.

## 📊 Tableau de bord Power BI

Le rapport Power BI anonymisé fournit une vision consolidée de l’activité, notamment :

- Le suivi du portefeuille de contrats
- Les indicateurs de chiffre d’affaires des contrats actifs
- Le suivi des paiements et des annulations
- L’analyse de la durée et du départ des contrats
- La comparaison entre les centres anonymisés
- Des filtres facilitant l’exploration opérationnelle

Le dépôt public contient uniquement un export PDF anonymisé. Le fichier Power BI original et les données de l’entreprise ne sont pas publiés.

## 💡 Recommandations métier

- Contacter de manière proactive les contrats présentant un risque plus élevé.
- Surveiller les profils contractuels associés aux courtes durées et aux annulations.
- Analyser le rôle et la rentabilité des remises.
- Mettre en place des alertes pour les contrats nécessitant un suivi commercial.
- Réentraîner et contrôler les modèles lorsque de nouvelles données deviennent disponibles.
- Collecter un nombre limité de variables clients pertinentes à l’aide de listes déroulantes courtes.
- Enregistrer les motifs d’annulation et de départ de manière homogène.
- Maintenir une validation humaine pour chaque décision commerciale.

## 📚 Livrables du projet

### 📓 Jupyter Notebook

Le notebook documente :

- Le regroupement et le nettoyage des données
- Les contrôles de qualité
- L’analyse exploratoire
- La préparation des variables
- La modélisation prédictive
- L’évaluation et l’interprétation des modèles

### 📊 Rapport Power BI

Le rapport anonymisé présente les principaux indicateurs opérationnels et analytiques au sein d’un tableau de bord clair.

### 🎨 Présentation Canva

La présentation explique la problématique de l’entreprise, la méthodologie, les résultats, les limites et les recommandations dans un format orienté métier.

## 📁 Structure du dépôt

```text
Self-Storage-Rental-Analysis/
├── README.md
├── README_FR.md
├── requirements.txt
├── .gitignore
├── notebooks/
│   └── self_storage_analysis.ipynb
├── powerbi/
│   └── powerbi_dashboard_anonymized.pdf
├── presentation/
│   └── self_storage_analysis_report.pdf
└── images/
    └── dashboard_overview.png
```

## 🔐 Confidentialité

Ce dépôt est destiné à une publication dans un portfolio.

Il ne contient pas :

- Les fichiers CSV ou Excel bruts de l’entreprise
- Les noms réels des centres
- Les noms des employés
- Les identifiants des contrats
- Le fichier Power BI original
- Les exports opérationnels confidentiels

Tous les documents publiés doivent être contrôlés et anonymisés avant leur mise en ligne.

## ⚠️ Utilisation responsable

Les modèles prédictifs identifient des régularités statistiques dans les données contractuelles disponibles. Ils ne doivent pas être utilisés pour prendre des décisions commerciales entièrement automatisées.

Les prédictions doivent toujours être examinées par une personne et associées à la connaissance opérationnelle de l’entreprise.

## 👩‍💻 Autrice

**Anaïs Fonvieille**

Projet d’analyse de données, de création d’un tableau de bord et de modélisation prédictive.
