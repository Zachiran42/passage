# Passage

[Télécharger l’APK](https://github.com/Zachiran42/passage/releases/latest/download/passage-0.1.0.apk) · [Versions](https://github.com/Zachiran42/passage/releases) · [Page du jeu](https://zachiran42.github.io/passage/)

Prototype Android natif hors ligne, sans publicité et sans permission. Android8+, APK universel. Licence MIT.

Trois traversées, portes périodiques. Maintiens et glisse le doigt pour guider le disque, puis relâche pour attendre. Passe par les ouvertures claires et vise la sortie en haut. Les détours dorés rapportent30points. Une collision arrête le mouvement et réduit seulement le bonus de sortie ; la partie peut continuer.

## Compiler
Configurer .toolchain.json à partir du modèle et définir MINIGAMES_KEYSTORE_PASSWORD dans l’environnement. scripts/build.ps1 prend une clé externe (-KeyStore) et son alias (-KeyAlias). Ne jamais publier les clés.

APK signé de développement ; aucun essai sur appareil physique effectué. Pause à la mise en arrière-plan. Le record est conservé localement ; la tentative en cours reste en mémoire tant que le processus vit.

## Dans Cercle

Dans « Ajouter depuis GitHub », coller `https://github.com/Zachiran42/passage`. La dernière Release contient un seul APK, signé, universel et sans permission Internet.

## Compilation

Copier `.toolchain.example.json` vers `.toolchain.json`, renseigner JDK21, Android SDK36 et Build Tools, puis définir `MINIGAMES_KEYSTORE_PASSWORD` dans l’environnement. Utiliser `scripts/build.ps1 -KeyStore C:/cles/jeu.keystore -KeyAlias votre-alias`. Garder les clés hors du dépôt.
