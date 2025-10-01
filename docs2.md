* Qu’est-ce qu’un APK ?

  C’est le fichier Android Package (APK).

  Comparable à un .exe sur Windows ou un .dmg sur macOS : il contient l’application prête à être installée.


* Différence debug vs release

  Debug APK : généré pendant le développement, non optimisé, contient des outils de debug (logs, inspection mémoire…).

  Release APK : optimisé et signé avec une clé de production, prêt à être publié sur le Play Store.


* assembleDebug

  C’est une tâche Gradle fournie par Android.

  Quand tu l’exécutes (ex. ./gradlew assembleDebug), elle :

      Compile ton code et tes ressources.

      Construit un APK debug.

      Dépose ce fichier dans app/build/outputs/apk/debug/app-debug.apk.