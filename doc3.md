

# Les concepts et outils de Jetpack Compose (le framework moderne d’Android pour construire des interfaces utilisateur déclaratives)
 
 - remember

  Sert à mémoriser un état (ex. un compteur, un texte saisi) tant que le composable reste en mémoire.

  Limite : si l’activité est détruite (ex. rotation d’écran ou retour arrière), la valeur est perdue.


- rememberSaveable

  Même principe que remember, mais en plus :

  il sauvegarde automatiquement la valeur dans un Bundle système,

  et la restaure après une recréation d’activité (rotation, changement de thème…).

  Donc : l’état survit aux changements de configuration.


- mutableStateOf

  Crée une valeur observable :

  Quand elle change, Compose redessine automatiquement les parties de l’UI qui en dépendent.

  C’est la base de la réactivité dans Compose.


 - Column

  Un conteneur qui empile ses enfants verticalement.

  Utile pour structurer ton interface (ex. TextField au-dessus d’un bouton).
  

 - Modifier

  Sert à configurer l’apparence et le comportement d’un composable.

  C’est une chaîne d’instructions :

    taille (fillMaxWidth()),

    marges (padding(16.dp)),

    bordures (border(1.dp, Color.Black)),accessibilité, clics (clickable { ... }), etc.