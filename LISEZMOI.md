# Lumen (version GitHub Pages)

Site de streaming 100 % statique : il tourne directement sur GitHub, sans serveur.

## Mise en ligne
1. Crée un dépôt GitHub (ex. `lumen`) et envoie-y tout le contenu de ce dossier.
2. Dépôt > **Settings** > **Pages** > *Deploy from a branch* > branche `main`, dossier `/ (root)` > **Save**.
3. Après 1-2 minutes, ton site est sur `https://TON-PSEUDO.github.io/lumen/`. Il marche sur PC et mobile (sur téléphone : « Ajouter à l'écran d'accueil »).

## Ajouter du contenu
1. Ouvre `…/admin.html`, crée catégories, titres et épisodes, puis **Télécharger catalog.json**.
2. Dans ton dépôt, remplace `catalog.json` par ce fichier (Add file > Upload files). Le site se met à jour tout seul.

## Où mettre les vidéos
- Petits fichiers (moins de 100 Mo) : dossier `videos/` du dépôt, lien `videos/mon-film.mp4`. Les affiches vont dans `posters/`.
- Gros fichiers : un hébergeur de fichiers, puis colle le lien direct du `.mp4` (Cloudflare R2, Bunny, ton propre serveur, Internet Archive pour du contenu qui s'y prête…).
- Format conseillé : MP4 en H.264 + AAC.

GitHub Pages n'est pas fait pour diffuser beaucoup de vidéo (site limité à 1 Go, trafic limité à environ 100 Go par mois) : ne mets pas les gros fichiers dans le dépôt. Mets uniquement des vidéos dont tu as les droits.
