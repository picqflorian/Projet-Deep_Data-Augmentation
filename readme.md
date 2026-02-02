# 🚀 Smart Data Augmentation & Model Patching

Ce projet explore l'impact de stratégies d'augmentation de données actives (Active Data Augmentation) sur l'entraînement de réseaux de neurones profonds (ResNet-18 sur CIFAR-10).

Il compare trois approches : **Baseline**, **Max Loss (Active Sampling)** et **Dynamic Curriculum**, et démontre comment l'augmentation de données peut corriger des biais de modèle (Model Patching).

## 📂 Structure du projet

Voici les deux notebooks principaux de ce dépôt :

### 1️⃣ `demo.ipynb` (Start Here / À lire) 👈
**C'est le notebook de présentation.**
* Il contient l'explication théorique, les visualisations des augmentations et l'analyse des résultats.
* Il charge les logs pré-enregistrés pour afficher les courbes de comparaison instantanément.
* **C'est le fichier destiné au lecteur.**

### 2️⃣ `main.ipynb` (Training Source)
**C'est le moteur d'entraînement.**
* Il contient tout le code lourd (Training Loops, Gestion du GPU, Sauvegardes).
* Il a été exécuté pour générer les modèles et les logs.
* *Note : Ne lancez ce notebook que si vous souhaitez ré-entraîner les modèles depuis zéro (prend plusieurs heures).*

## 📊 Dossier `results/`
Ce dossier contient les fichiers `.json` (logs d'entraînement) et `.pth` (poids des modèles) générés par `main.ipynb` et utilisés par `demo.ipynb` pour l'affichage.

