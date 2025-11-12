# kaggle_A-d_Al-Adha_2025
# 🐏 Sheep Classification Challenge 2025  

![Kaggle](https://img.shields.io/badge/Kaggle-Competition-blue)  
![Score](https://img.shields.io/badge/Score-0.92223-success)  
![Framework](https://img.shields.io/badge/PyTorch-🔥-orange)  

> **Compétition Kaggle :** [Sheep Classification Challenge 2025](https://www.kaggle.com/competitions/sheep-classification-challenge-2025)  
> **Score final :** 🏆 **0.92223**

---

## 📖 Contexte  

Dans le cadre de **l’Aïd al-Adha 2025**, cette compétition visait à développer un modèle de **vision par ordinateur** capable de reconnaître la **race d’un mouton** à partir d’une image.  
Le dataset contenait des images de **7 races ovines** différentes, telles que *Naeimi*, *Najdi*, *Harri*, etc.  

---

## 🧠 Approche & Méthodologie  

### 1️⃣ Préparation des données  
- Analyse exploratoire (distribution des classes, inspection visuelle des images).  
- Nettoyage et redimensionnement des images.  
- **Data augmentation** : flips, rotations, crops, brightness, etc.  
- Normalisation selon les statistiques d’ImageNet.

### 2️⃣ Modélisation  
- Framework : **PyTorch**  
- Modèle : **CNN pré-entraîné (ResNet / EfficientNet)**  
- Fine-tuning sur le dataset spécifique.  
- Remplacement de la couche fully-connected finale pour **7 classes**.  

### 3️⃣ Entraînement  
- Split du dataset : **80% entraînement / 20% validation**  
- Callbacks : *early stopping*, *learning rate scheduler*  
- Optimiseur : Adam / SGD  
- Suivi de la **loss** et de l’**accuracy** sur chaque epoch.

### 4️⃣ Optimisation  
- Hyperparamètres testés : *learning rate*, *batch size*, *nombre d’époques*, *data augmentations*  
- Validation croisée (*k-fold*) pour robustesse.  
- Sauvegarde automatique du **meilleur modèle** selon la performance sur validation.

### 5️⃣ Évaluation  
- Génération des prédictions sur l’ensemble de test.  
- Formatage du fichier de soumission selon le template Kaggle.  
- Score obtenu sur le leaderboard public : **0.92223**

---

## 📂 Structure du projet  


