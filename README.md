Création de Schéma Entité-Association (Méthode Merise) avec l'outil Looping 

## Objectif
Ce modèle GitHub permet d'utiliser **Looping**, l'outil de modélisation **Merise**, directement depuis **GitHub Codespaces**, sans installation locale.  
Il est conçu pour les cours de **BTS SIO SLAM** et toute formation en **conception de bases de données**.

## Utilisation rapide
1. Ouvre ce dépôt dans **GitHub Codespaces**.
2. Ouvre le port `80` et clique sur **Open in Browser**.
3. Une interface graphique LXDE s’affiche.
4. Double-clique sur **“Looping (Merise)”** pour lancer le logiciel.
5. Crée ton **MCD**, **MLD**, et **script SQL** directement depuis le cloud !

## Sauvegarde
Enregistre tes fichiers dans le dossier `models/` — ils seront versionnés par Git.

## Comment mettre à jour son dépôt Github distant depuis son PC local
Travaux pratiques
- Téléchargement d'un client GIT pour Windows en local : Git Bash ( aussi appelé "GIT for Windows" )
- Récupération de l'URL du dépôt distant via Github Codespace 
- Choisir un répertoire local qui stockera le clone du répertoire distant
- Clic droit + "Autres options"
- Clic droit dans ce répertoire + "Open GIT Bash here"
- git clone <URL_DEPOT_GITHUB>
- git add .       
    ( pour prendre en compte des modifications effectuées dans le répertoire local)
- git commit -m "MESSAGE_INDIQUANT_CE_QUI_A_ETE_MODIFIé_DANS_REPERTOIRE_LOCAL"
- git push 
   (pour mettre à jour le répertoire (dépôt GITHUB) distant

## Outils intégrés
- **Looping.exe** (via Wine)
- **LXDE Desktop**
- **noVNC** (port 6080)
- **GitHub Codespaces**

---

# TP – Schéma Entité-Association (Méthode Merise)

## Contexte

Une application de **vente en ligne (e-commerce)** doit être modélisée à l’aide de la méthode **Merise**.  
L’objectif est de produire un **Modèle Conceptuel de Données (MCD)** à partir de l’énoncé fourni.

---

## Énoncé

Une société de vente en ligne souhaite gérer les commandes passées par ses clients.  
Chaque client peut passer plusieurs commandes.  
Une commande contient plusieurs produits, avec pour chaque produit une quantité et un prix au moment de la commande.  
Chaque produit appartient à une seule catégorie.  
Certains produits sont proposés par plusieurs fournisseurs.  
Chaque fournisseur peut livrer plusieurs produits.  
Enfin, un client peut recommander un autre client lors de son inscription.

- Les élèves ont identifié les 5 entités : Client , Commande , Produit , Catégorie et Fournisseur .
- Un identifiant unque a été défini pour chaque entité
- Les attributs de l'entité Produit ont été définis (avec l'outil looping) : libelle , quantité , prix (avec le type adéquat : texte, entier , réel
---

## Travail demandé

### Exercice 1 – Identification des entités

1. Liste les **entités** nécessaires à la modélisation du système.  
2. Justifie brièvement le choix de chaque entité.

### Exercice 2 – Attributs des entités

1. Pour chaque entité identifiée, propose une liste d’**attributs**.  
2. Indique pour chaque entité son **identifiant**.  
3. Précise si certains attributs te semblent facultatifs.

### Exercice 3 – Associations

1. Identifie les **associations** entre les entités.  
2. Donne un **nom explicite** à chaque association.  
3. Indique les entités reliées par chaque association.

### Exercice 4 – Cardinalités

1. Détermine les **cardinalités minimales et maximales** pour chaque association.  
2. Justifie chaque cardinalité à partir de l’énoncé.

### Exercice 5 – Cas particuliers

1. Identifie les associations portant des **attributs propres**.  
2. Indique si un **identifiant composite** est nécessaire.  
3. Justifie ton choix.

### Exercice 6 – Modélisation avec Looping

1. Réalise le **MCD complet** à l’aide de l’outil Looping.  
2. Vérifie la cohérence globale du modèle.  
3. Sauvegarde le fichier Looping dans le dossier `models/`.

---

## Rendu attendu

- Un **fichier Looping (.loo)** contenant le MCD.  
- Le modèle doit être **lisible**, **cohérent** et **conforme à la méthode Merise**.
