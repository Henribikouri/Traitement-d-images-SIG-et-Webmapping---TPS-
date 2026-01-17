# 🖼️ TPS de Traitement d'Images Numériques (Chapitres 1-7)

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Toolkit](https://img.shields.io/badge/Libraries-NumPy%20|%20Pillow%20|%20Matplotlib-green.svg)

CeS TPs  implémentent une chaîne complète de traitement d'images, allant de la manipulation de bas niveau (pixels) à l'extraction de connaissances (segmentation et morphologie). Il a été conçu comme socle technique pour des applications en **SIG** et **Webmapping**.

---
Auteur : Henri BIKOURI
## 🚀 Architecture du Projet

Le projet est organisé de manière modulaire pour faciliter l'exécution et le test de chaque algorithme :

* **`entree/`** : Répertoire central contenant les images sources de test.
* **`Chap1/` à `Chap7/`** : Dossiers thématiques regroupant les scripts Python (.py).
* **`sortie/`** : Sous-répertoires au sein de chaque chapitre contenant les fichiers sauvegardés après traitement.

---

## 🛠️ Contenu des Chapitres

1.  **Chapitre 1 : Fondements** - Manipulation des formats PGM/PPM et profil d'intensité.
2.  **Chapitre 2 : Ponctuel** - Histogrammes, étirement de contraste, égalisation et interpolation (bilinéaire/bicubique).
3.  **Chapitre 3 : Convolution** - Filtres de lissage (Moyenneur, Gaussien) et filtre Médian (anti-bruit).
4.  **Chapitre 4 : Fréquentiel** - Transformée de Fourier (DFT) et filtres Notch (réjecteurs de bande).
5.  **Chapitre 5 : Contours** - Opérateurs de Sobel, Prewitt, Laplacien et seuillage par Hystérésis.
6.  **Chapitre 6 : Segmentation** - Méthode d'Otsu, K-means et Ligne de partage des eaux (Watershed).
7.  **Chapitre 7 : Morphologie** - Érosion, Dilatation, Ouvertures/Fermetures et Code de Freeman.

---

## 🚦 Protocole de Test

### 1. Installation des dépendances
Le projet nécessite un environnement Python 3 avec les bibliothèques suivantes :
```bash
pip install -r requirements.txt
```
---

## 🧪 Protocole de Test & Validation

### 1. Préparation des Données
Avant de lancer les scripts, assurez-vous que vos images de test sont placées dans le dossier racine `entree/`. Les scripts sont configurés par défaut pour lire :
* `entree/henri1.png` (ou format .jpg/ .pgm)
* `entree/henri2.png` (pour les opérations arithmétiques du Chapitre 2)

### 2. Flux de Traitement (Workflow)
Chaque TP suit un cycle d'exécution standardisé :
1. **Chargement** : Lecture du fichier depuis `/entree`.
2. **Prétraitement** : Conversion systématique en niveaux de gris (pour les algos de contours/segmentation).
3. **Traitement** : Application de l'algorithme (ex: Transformation de Fourier ou Seuil d'Otsu).
4. **Visualisation** : Affichage via une fenêtre interactive Matplotlib.
5. **Sauvegarde** : Exportation automatique du résultat dans le dossier `sortie/` du chapitre concerné.



### 3. Exemple de Test : Détection de Contours (Chapitre 5)
Pour vérifier la robustesse de l'algorithme de Sobel :
```bash
# Se placer à la racine du projet
python Chap5/tp5sobel.py
