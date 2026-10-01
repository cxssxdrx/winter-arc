# Winter Arc : installation sur iPhone (environ 10 minutes, une seule fois)

## 1. Mettre l'app en ligne (GitHub Pages, gratuit)
1. Crée un compte sur github.com si tu n'en as pas.
2. Clique sur **New repository**, nomme-le `winter-arc`, choisis **Public**, puis **Create repository**.
3. Clique sur **uploading an existing file** et glisse **tout le contenu** du dossier : `index.html`, `manifest.webmanifest`, `sw.js` et le dossier `icons`. Valide avec **Commit changes**.
4. Va dans **Settings → Pages**. Sous Source, choisis **Deploy from a branch**, puis la branche `main` et le dossier `/ (root)`, et clique sur **Save**.
5. Après 1 à 2 minutes, l'app est en ligne à l'adresse `https://TON-PSEUDO.github.io/winter-arc/`.

Le dépôt contient uniquement le code. Ta clé API et tes données restent sur ton téléphone.

## 2. L'installer sur l'iPhone
1. Ouvre l'adresse dans **Safari** (pas Chrome).
2. Touche **Partager**, puis **Sur l'écran d'accueil**, puis **Ajouter**.
3. Ouvre l'app depuis l'icône Winter Arc : elle s'affiche en plein écran, sans barre Safari.

## 3. Relier Garmin
L'app lit tes données Garmin via **Intervals.icu**, qui est déjà relié à ta montre.
1. Sur intervals.icu, va dans **Settings**, puis **Developer Settings** (tout en bas), et copie ton **API key**.
2. Dans l'app, colle la clé, laisse l'ID athlète à `0`, puis touche **Connecter**.
3. Vérifie que les **pas** remontent bien : sur intervals.icu, la page Wellness doit afficher les pas du jour. Si ce n'est pas le cas, active l'import des données wellness dans les réglages de la connexion Garmin d'Intervals.icu.

## Fonctionnement au quotidien
- **Synchro automatique** à chaque ouverture de l'app, puis toutes les 15 minutes tant qu'elle est ouverte. Le circuit est le suivant : la montre envoie à Garmin Connect, qui envoie à Intervals.icu, qui envoie à l'app. Compte quelques minutes de délai.
- **Sport, pas et sommeil** se cochent tout seuls. Si Garmin n'a rien remonté (montre oubliée), touche la ligne pour valider manuellement.
- **Les cases d'hier** restent cochables jusqu'à 10 h.
- **Sauvegarde** : dans Réglages, choisis Exporter, puis enregistre le fichier dans Fichiers ou iCloud Drive. Fais-le environ une fois par semaine. Supprimer l'app de l'écran d'accueil efface ses données.

## Mettre l'app à jour
Remplace `index.html` dans le dépôt GitHub. L'app récupère la nouvelle version à la prochaine ouverture (ferme-la et rouvre-la deux fois).
