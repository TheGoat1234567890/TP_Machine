# TP_Machine

Partie 1 : Analyse Exploratoire des Données (EDA)

1.1 Vue d'ensemble des données :

Ce sont les caractéristiques d'une personne. Cela commence avec une ID unique pour reconnaitre une personne parmis tant d'autre, ensuite il y a les caractéristiques comme : le genre, l'age, la taille (cm), le poids (kg), tour de taille (cm), la vue gauche, la vue droite, l'audition gauche, l'audition droite, hémoglobine, protéine urinaire, créatine sérique, AST, AST, Gtp, Oral, caries dentaires, tartre et tabagisme.

Grace à la fonction describe(), on peut voir qu'il y a 55702 entrées dans le jeu de données.

Oui il contient 6 valeurs nulles dans l'age et 6 dans le poids. 

1.2 Statistiques descriptives :

Pour les fumeurs, la moyenne d'age est de 43.560813, la moyenne de taille est de 169.435401 cm, et le poids de 70.959376.

Oui il y a quelqu'un qui a 40 000 ans!!

L'ecart type de l'hemoglobine est de 1.137560 chez les fumeurs et de 1.564476 en globale.

1.3 Distribution de la donnée :

il y a plus d'homme qui fume que de femme. Presque 20000 (19597) pour les hommes contre environ 1000 (859).

1.4 Analyse de corrélation :

Le problème est qu'il y a des valeurs manquantes et des string.


Partie 2 : Data pre-processing

2.1 Gestion des Valeurs Manquantes :

J'ai choisi d'imputer les valeurs manquantes avec la moyenne pour les variables numériques.Cette méthode permet de conserver toutes les observations en remplaçant les valeurs manquantes par des valeurs représentatives, minimisant ainsi la perte d'information.

Les données vont etre plus reprensentative, mais vont se rapprocher de la moyenne evidemment. 

2.2 Encodage des catégories

Voici une autre méthode : traitement des valeurs aberrantes : Identifier et traiter les valeurs aberrantes pour éviter qu'elles n'affectent de manière disproportionnée le modèle.

1.4 Analyse de corrélation :

Je ne comprend pas, j'ai une matrice 2x2.


Partie 3 :

3.1 Création de jeu de test et d'entraînement

J'ai utilisé 80% des données pour l'entraînement et 20% pour le test.

Il est important de diviser cela en test et en entrainement, car le modele s'entraine sur les 80 pourcents qu'on lui donne et ensuite on verifie avec les autres données (Test) qui sont inconnues. Ainsi on peut voir si notre "prediction" correle ou non. 

3.2 Entraînement d'un modèle simple : LogisticRegression

Résultats du Modèle sur le Jeu de Test :

Accuracy: 0.741315860335697
Precision: 0.6540750323415265
Recall: 0.6206727228087405
F1 Score: 0.636936255983875

3.3 Entraîner et ajuster les paramètres de plusieurs modèles

L'ajustement des hyperparamètres permet d'optimiser les performances des modèles en trouvant les configurations qui minimisent l'erreur de prédiction sur l'ensemble de validation croisée. Cela peut améliorer significativement la précision, le rappel et le score F1 des modèles ( je n'ai pas réussi à faire les modèles, mais je me suis renseigné sur la question)

Donc je n'ai pas réussi à faire un seul modèle, mais je sais que le modèle ayant les meilleures performances globales sera celui avec les scores les plus élevés en accuracy, recall, et F1-score.










