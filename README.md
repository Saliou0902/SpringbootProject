
# Mise en place de l’environnement

## Introduction:

Le projet consiste à mettre en place une solution de détection d’objets en temps réel à partir de flux vidéo fournis par des caméras IP. L’objectif principal est d'améliorer la sécurité et la surveillance des lieux en permettant la détection automatique d'objets ou d'individus spécifiques dans l'environnement filmé. Ce système est conçu pour fonctionner en temps réel, ce qui permet de réagir rapidement à des événements de sécurité potentiels.

Ce projet est une solution efficace pour la surveillance automatiée , en temps réel, avec les résultats affichés instantanément sur une inteface.

## Prérequis pour les différentes versions:

### Environnement logiciel:

- Systeme d’exploitation: Recommande Linux ou windows (selon ton infrastructure).
- Python : python 3.10.12

### Bibliotheques python:

Les dépendances à installer via `pip` sont spécifiées dans le fichier `requirements.txt`. Voici les principales bibliothèques :

- **deep-sort-realtime==1.3.2** : Utilisé pour le suivi des objets détectés en temps réel.
- **filterpy==1.4.5** : Une bibliothèque pour les filtres de Kalman et d'autres techniques d'estimation.
- **numpy==1.26.4** : Une bibliothèque pour les calculs scientifiques et la manipulation de matrices.
- **opencv-python==4.10.0.84** : Utilisé pour le traitement d'images et la capture vidéo depuis des flux IP.
- **pandas==2.2.2** : Pour la manipulation de données.
- **pillow==10.4.0** : Traitement d'images (principalement pour les formats d'image).
- **scikit-image==0.24.0** : Outils pour le traitement d'images.
- **scipy==1.14.1** : Fonctions mathématiques avancées, nécessaires pour certaines méthodes de traitement d'images.
- **seaborn==0.13.2** : Bibliothèque pour la visualisation de données (peut-être utile pour analyser les résultats).
- **ultralytics==8.2.94** : Contient les implémentations de YOLOv8 pour la détection d'objets.

## Comment lancer le projet?

OPTION 1 : EN LOCAL

1. **Cloner le dépôt** :
   - Télécharge le projet depuis GitHub ou un autre dépôt :

   ```bash
   git clone https://github.com/sakanokoh/TransDic2ShirikiEye
   cd project
   ```
   
2. **Installer les dépendances** :
   - Utilise la commande suivante pour installer les dépendances à partir du fichier `requirements.txt` :

   ```bash
   pip install -r requirements.txt
   ```
   
3. **Lancer l'application** :
   - Une fois les dépendances installées, tu peux exécuter l'application :

   ```bash
   python app.py
   ```
   
   - Assure-toi que le fichier `app.py` ou le fichier principal du projet contient la logique de détection d'objets et le traitement du flux des caméras IP.

OPTION 2: EXECUTION DANS UN ENVIRONNEMENT VIRTUEL

1. **Créer un environnement virtuel** :
   - Il est recommandé de créer un environnement virtuel pour isoler les dépendances du projet :

   ```bash
   python3 -m venv myenv
   ```
   
2. **Activer l'environnement** :
   - **Sous Linux/macOS** :

   ```bash
   source myenv/bin/activate
   ```
   
   - **Sous Windows** :

   ```bash
   myenv\Scripts\activate
   ```
   
3. **Installer les dépendances** :
   - Une fois l'environnement activé, installe les dépendances :

   ```bash
   pip install -r requirements.txt
   ```
   
4. **Lancer l'application** :
   - Exécute le fichier principal :
