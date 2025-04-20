# Analyse Prédictive du Turnover RH

Ce projet vise à analyser et prédire le turnover des employés à l’aide d’un modèle d’intelligence artificielle appliqué à un dataset RH. Utilisant un dataset Kaggle (38 colonnes, ~1470 lignes), il identifie les facteurs clés du turnover (e.g., surcharge de travail, département) et propose des solutions stratégiques pour améliorer la rétention. Conforme aux exigences RGPD, il met en avant une approche éthique de l’IA.

## Objectifs
- Identifier les principaux facteurs de départ des employés (Attrition).
- Développer un modèle prédictif précis pour anticiper les risques de turnover.
- Fournir des visualisations et KPIs actionnables pour les équipes RH.

## Méthodologie
- **Données** : Dataset Kaggle HR Analytics, nettoyé avec pandas.
- **Préparation** : Utilisation de SMOTE pour équilibrer les données déséquilibrées.
- **Modélisation** : Comparaison de Random Forest et XGBoost, choix de XGBoost (80 % d’accuracy).
- **Visualisation** : Barplot Seaborn des 10 variables les plus influentes (OverTime, Department_R&D,...).
- **Éthique** : Exclusion des colonnes sensibles (Gender, MaritalStatus, EmpID) pour conformité RGPD.

## Livrables
- `Projet_Turnover_RH_Python_Francais.ipynb` : Notebook Jupyter contenant le code complet (nettoyage, modélisation, visualisation).

## Installation
Pour exécuter le notebook, installez les dépendances suivantes et lancez Jupyter :
```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost imbalanced-learn
jupyter notebook Projet_Turnover_RH_Python_Francais.ipynb
```

## Contact
Johanna Fokui  
[LinkedIn, si applicable]  
Pour toute question ou collaboration, n’hésite pas à me contacter !

## Remarque
Ce projet est réalisé dans un cadre académique et professionnel pour explorer l’application de l’IA aux Ressources Humaines, avec un focus sur l’éthique et l’impact RH.
```
