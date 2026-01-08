# Module 4 Brief 2

Ce projet explore différentes techniques de Machine Learning pour la classification d'images de chiffres manuscrits. 

Il compare des méthodes classiques (Clustering, Régression Logistique) sur des données basse résolution avec des méthodes de Deep Learning (CNN) sur des données plus complexes.

## Datasets Utilisés

1.  **Sklearn Digits (8x8 pixels)** :
    *   Utilisé pour l'analyse exploratoire, la PCA, le K-Means et la Régression Logistique.
    *   Images très basse résolution, rapides à traiter.
    *   64 caractéristiques (features) par image.

2.  **Keras MNIST (28x28 pixels)** :
    *   Utilisé pour l'entraînement du CNN.
    *   Images plus détaillées, standard de l'industrie pour les benchmarks de vision.
    *   784 caractéristiques par image (traitées comme une grille 28x28x1).

## éthodologie

Le notebook est structuré en plusieurs étapes logiques :

1.  **Prétraitement** : Normalisation des pixels (mise à l'échelle entre 0 et 1) pour faciliter la convergence des algorithmes.
2.  **Réduction de Dimension (PCA)** : Projection des données 8x8 (64 dimensions) en 2 dimensions pour visualiser la séparabilité des classes.
3.  **Clustering (K-Means)** : Tentative de regroupement non supervisé. La méthode du coude est utilisée pour valider le choix de k=10.
4.  **Régression Logistique** : Modèle linéaire simple appliqué aux données 8x8 aplanies.
5.  **CNN (Convolutional Neural Network)** : Modèle profond appliqué aux données 28x28, capable d'apprendre des filtres spatiaux (bords, formes).

## Installation 

```bash
pip install -r requirements.txt
```
