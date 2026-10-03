# NoteCad

NoteCad est un prototype d’atelier de dessin et de conception 2D/3D. L’interface est en français et le prototype fonctionne hors ligne.

## Télécharger

Les téléchargements seront ajoutés dans [Releases](https://github.com/cissmomo08-byte/NoteCad/releases) après la première compilation. Les fichiers prévus sont :

- **Windows** : installateur et version portable `.exe`.
- **macOS** : image `.dmg` universelle pour Mac Intel et Apple Silicon.
- **Linux** : `.AppImage` portable.
- **Navigateur** : `NoteCad.html`, utilisable hors ligne.

La première version installable n’est pas encore publiée. Les compilations automatiques seront vérifiées avant de publier les téléchargements.

## Lancer le prototype web

Ouvre `index.html` dans un navigateur récent. Pour une application de bureau : installe Node.js 22.12 ou plus récent, puis lance `npm install` et `npm start` dans ce dossier.

## Compiler

- `npm run dist:win` : Windows x64.
- `npm run dist:mac` : macOS universel.
- `npm run dist:linux` : Linux x64.

Les instructions de distribution sont dans [DISTRIBUTION.md](DISTRIBUTION.md). La confidentialité est décrite dans [PRIVACY.md](PRIVACY.md).

## Licence

Aucune licence de réutilisation n’est encore définie. Le dépôt est public pour héberger le projet et les téléchargements ; cela n’autorise pas la réutilisation du code sans accord.
