# Dolphin project :


- Traitement des données - Récupérer la liste des actifs au 1er juin 2016
  - Conversion des différentes valeurs de chaque actif en le type approprié pour pouvoir les manipuler.
  - Conversion de toutes les valeurs monétaires en euros à l&#39;aide de notre tableau de taux de conversion.
  - Conversion de la liste des actifs en un Data Frame


- Sélection des actifs et leurs quantités
  - Matrice de corrélations sur tous les actifs
  - KMeans pour répartir en groupes d&#39;actifs fortement corrélés
    - Variation du nombre de groupes d&#39;actifs entre 15 et 40
    - Sélection de l&#39;actif avec le meilleur sharpe de chaque groupe
  - Descente de gradient pour trouver la quantité optimale pour chaque actif sélectionné en maximiser le ratio sharpe avec les contraintes suivantes :
    - NAV de chaque actif au sein du portefeuille entre 1% et 10% du NAV du portefeuille
    - Montant des actifs de type &quot;stock&quot; supérieur à 50% du montant total du portefeuille


- Validation de notre portefeuille
  - Vérification du respect des contraintes
  - Publication de la composition d&#39;actifs dans notre portefeuille GROUPE 10
  - Comparaison du sharpe entre notre portefeuille et le portefeuille de référence
