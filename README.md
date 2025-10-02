# HelloCounter

## 1) Générer l'APK

### En utilisant Android Studio

1. Ouvrez votre projet dans **Android Studio**.
2. Allez dans **Build → Build Bundle(s) / APK(s) → Build APK(s)**.
3. Attendez que la construction se termine.
4. Le fichier APK sera généré à :

```
app/build/outputs/apk/debug/app-debug.apk
```

---

### En utilisant la ligne de commande (optionnel)

Depuis la racine de votre projet, exécutez :

```bash

# Windows
gradlew assembleDebug
```

L'APK sera généré au même emplacement :

```
app/build/outputs/apk/debug/app-debug.apk
```

---

## 2) Installer l'APK

### Sur un appareil physique

1. Copiez l'APK sur votre appareil Android.
2. Activez **l'installation à partir de sources inconnues** dans les paramètres système.
3. Ouvrez le fichier APK et confirmez l'installation.

### En utilisant ADB (Android Debug Bridge)

Si vous avez ADB installé, exécutez :

```bash

adb install -r app/build/outputs/apk/debug/app-debug.apk
```

* `-r` → remplace l'installation précédente si l'application est déjà installée.

---

## 3) Exécuter l'Application

Après l'installation, trouvez l'icône de l'application (par exemple **HelloCounter**) sur votre appareil ou émulateur et ouvrez-la.

---