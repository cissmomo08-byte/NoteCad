# Préparer une version téléchargeable de NoteCad

## Formats configurés

- Windows 64 bits : installateur `.exe` et version portable `.exe`.
- macOS : image `.dmg` et archive `.zip` universelles pour Mac Intel et Apple Silicon.
- Linux 64 bits : `.AppImage` et `.deb`.

La chaîne de compilation est configurée dans `package.json` et `.github/workflows/release.yml`. Une étiquette Git de version au format `v0.2.0` déclenchera la création des paquets dans GitHub Actions et préparera un brouillon de version GitHub avec les fichiers à télécharger. Le brouillon doit être vérifié et publié depuis GitHub avant que les liens soient publics.

## Compilation locale

Installer Node.js 22.12 ou plus récent, puis exécuter `npm install`. Pour lancer l’application : `npm start`. Pour créer les fichiers du système courant : `npm run dist`. Les scripts `dist:mac`, `dist:win` et `dist:linux` créent chaque format sur un runner du système correspondant.

## Avant une publication publique

1. Héberger ce projet dans un dépôt GitHub appartenant à l’éditeur.
2. Vérifier les installateurs sur chaque système.
3. Configurer la signature de code et la notarisation macOS/Windows avec les identifiants de l’éditeur.
4. Publier une URL permanente vers `PRIVACY.md`.
5. Examiner le brouillon de version et publier ses téléchargements.

Le compte Apple Developer, la signature Windows et les comptes des boutiques sont indépendants de ce dépôt. Ils ne sont pas configurés dans le projet.
