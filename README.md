# 🖼️ TPS de Traitement d'Images Numériques (Chapitres 1-7)
Auteur : Henri BIKOURI
![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Toolkit](https://img.shields.io/badge/Libraries-NumPy%20|%20Pillow%20|%20Matplotlib-green.svg)

CeS TPs  implémentent une chaîne complète de traitement d'images, allant de la manipulation de bas niveau (pixels) à l'extraction de connaissances (segmentation et morphologie). Il a été conçu comme socle technique pour des applications en **SIG** et **Webmapping**.

---

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
