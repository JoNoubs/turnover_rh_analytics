# Analyse Prédictive du Turnover RH
# Analyse Prédictive du Turnover RH

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

**Par Johanna Grace Fokui Noubi**

Ce projet analyse les **départs d’employés** à l’aide de l’intelligence artificielle, en exploitant le dataset **[Kaggle HR Analytics](https://www.kaggle.com/datasets/anshika2301/hr-analytics-dataset)** (38 colonnes, 1480 lignes). Il combine **exploration de données**, **modélisation prédictive**, et **recommandations RH** pour identifier les facteurs clés du turnover (surcharge de travail, salaire, relation managériale) et proposer des stratégies de rétention. Conforme au **RGPD**, il exclut les données sensibles (Gender, MaritalStatus, EmpID) pour une IA éthique et inclusive.

## Contexte
Le turnover affecte la performance, la culture d’entreprise, et le bien-être des employés. Ce projet explore comment l’IA peut anticiper les départs, fournir des insights exploitables, et promouvoir une gestion responsable des données RH.

## Objectif
- Identifier les **facteurs clés** influençant le départ des employés (Attrition).
- Développer un **modèle prédictif** précis pour anticiper le turnover.
- Fournir des **visualisations** et **analyses** pour orienter les décisions RH.

## Contenu du projet
- **`Projet_Turnover_RH_Johanna.ipynb`** : Notebook Jupyter incluant :
  - **Exploration et nettoyage** : Gestion des doublons et valeurs manquantes avec pandas sur le dataset Kaggle.
  - **Visualisations exploratoires** : Graphiques Seaborn/Plotly pour analyser satisfaction, ancienneté, surcharge, départements.
  - **Modélisation prédictive** : Test de Random Forest, SMOTE + Random Forest, et XGBoost (~86% accuracy).
  - **Analyse des variables** : Identification des facteurs influents (OverTime, MonthlyIncome, etc.).
  - **Réflexion éthique** : Conformité RGPD, gestion des biais, anonymisation.

## Outils utilisés
- **Python**, **Jupyter Notebook**
- **Bibliothèques** : `pandas`, `numpy`, `matplotlib`, `seaborn`, `plotly`, `scikit-learn`, `xgboost`, `imbalanced-learn`

## Installation
Pour exécuter le notebook, installez les dépendances suivantes et lancez Jupyter :
```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost imbalanced-learn
jupyter notebook Projet_Turnover_RH_Python_Francais.ipynb
```

## Principales observations
1. **Surcharge de travail** : `OverTime_Yes` domine tous les modèles, signalant un besoin urgent d’équilibre vie pro/perso.
2. **Salaire** : `MonthlyIncome` est clé dans Random Forest, soulignant l’importance de la reconnaissance financière.
3. **Statut célibataire** : `MaritalStatus_Single` indique une mobilité accrue, surtout dans les modèles équilibrés.
4. **Relation managériale** : `YearsWithCurrManager` montre qu’un encadrement stable réduit les départs.
5. **Âge indirect** : `Age` est corrélé à `TotalWorkingYears` et `YearsAtCompany`, mais moins prédictif seul.
6. **Rôles à risque** : `Department_Sales`, `Department_R&D`, `JobRole_Sales Representative`, et `BusinessTravel_Frequently` sont plus exposés.

## Modélisation
- **Random Forest** : Robuste, mais limité par le déséquilibre des classes (16% de départs).
- **SMOTE + Random Forest** : Améliore la détection des départs rares.
- **XGBoost** : Modèle optimal (~86% accuracy), capturant les interactions complexes.

## Résultats
- **Précision** : ~86% avec XGBoost après SMOTE, équilibrant précision et rappel.
- **Variables influentes** : Cohérentes avec les observations terrain (OverTime, MonthlyIncome, YearsWithCurrManager).
- **Impact** : Prédictions fiables pour identifier les employés à risque, intégrables dans des outils RH.

## 💡 Recommandations RH
- Réduire les **heures supplémentaires** via une meilleure gestion des charges.
- Soutenir les **jeunes talents** (<3 ans d’ancienneté) avec un accompagnement renforcé.
- Valoriser les **managers** pour des relations stables.
- Accompagner les **commerciaux** et rôles R&D à risque.
- Intégrer la **satisfaction** (`JobSatisfaction`) comme KPI dans les tableaux de bord RH.

## Limites
- Dataset fictif (Kaggle), limitant l’application directe.
- SMOTE peut introduire du bruit dans les données synthétiques.
- Nécessite une intégration dans des systèmes RH pour un usage opérationnel.

## Cas d’usage
- **Prédiction temps réel** : Alerter sur les risques de départ.
- **Tableaux de bord** : Visualiser les KPIs (turnover, satisfaction) dans Power BI.
- **Stratégies ciblées** : Adapter les politiques RH aux profils à risque.

## Contributions
Les contributions sont encouragées ! Pour proposer des améliorations :
1. Forkez ce dépôt.
2. Créez une branche (`git checkout -b feature/amélioration`).
3. Soumettez une pull request avec une description claire.

## Auteure
**Johanna Fokui**  
Étudiante en MSc Intelligence Artificielle & Data Science @ Aivancity  
[LinkedIn](https://www.linkedin.com/in/johanna-grace-fokui-noubi-18006022b/)  
[GitHub](https://github.com/JoNouba)  
[Portfolio](https://jonoubs.github.io)  
Pour toute question, suggestion ou collaboration, contactez-moi !

---

> Réalisé dans un cadre personnel, ce projet reflète une approche **technique**, **éthique**, et **humaine** de l’IA appliquée aux Ressources Humaines.

