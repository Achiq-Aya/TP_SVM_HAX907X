# TP SVM - Support Vector Machines

**Cours :** HAX907X - Apprentissage Statistique  
**Année :** 2025/2026  
**Université de Montpellier**

## Auteur
Achiq Aya

## Description

Ce projet contient le code et le rapport du TP sur les Support Vector Machines (SVM). On explore différents aspects des SVM : classification sur Iris, reconnaissance de visages, impact des variables de nuisance et réduction de dimension par PCA.

## Structure du projet
TP_SVM_HAX907X/
├── README.md              # Ce fichier
├── .gitignore
├── rapport.tex            # Rapport LaTeX
├── rapport.pdf            # Rapport compilé
├── images/                # Figures pour le rapport
│   ├── iris_classification.png
│   ├── accuracy_vs_C.png
│   └── ...
└── src/                   # Scripts Python
├── svm_source.py      # Fonctions utilitaires
├── svm_iris.py        # Q1-Q2: Dataset Iris
└── svm_face.py        # Q4-Q6: Classification de visages

## Environnement Python

**Dépendances requises :**
```bash
numpy
matplotlib
seaborn
scikit-learn
```
**Installation :**
```bash
pip install numpy matplotlib seaborn scikit-learn
```
## Compilation du rapport

Le rapport est écrit en LaTeX. Pour le compiler :
```bash
pdflatex rapport.tex
pdflatex rapport.tex  # Deux fois pour les références
```
Ou utilisez Overleaf en important rapport.tex et le dossier images/.

## Résultats principaux

- **Iris (Q1-Q2)** : 66% d'accuracy avec noyau linéaire et polynomial (degré=1)
- **Visages (Q4)** : 89.5% d'accuracy avec C=0.0001
- **Variables de nuisance (Q5)** : chute de 90.5% à 53% avec 300 variables aléatoires
- **PCA (Q6)** : amélioration limitée (variance 88%, score 55%)

## Références

- Scikit-learn : https://scikit-learn.org/stable/modules/svm.html
- Dataset LFW : http://vis-www.cs.umass.edu/lfw/
- Vapnik, V. N. (1998). Statistical learning theory. Wiley.