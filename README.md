# Catalogue Emballages — Cloudflare Pages

Site statique en français, sans nom de société, avec 6 produits, prix HT et PDF.

## Méthode 1 — Cloudflare Pages (sans GitHub)
1. Décompressez le fichier ZIP téléchargé.
2. Cloudflare Dashboard → Workers & Pages → Create → Pages → Upload assets (or Direct Upload).
3. Uploadez **le dossier contenant `index.html`, `catalogue/`, `assets/`**, ou le ZIP si l'interface le permet.
4. Déployez. Le site est accessible à `https://votre-projet.pages.dev/catalogue/`.

## Méthode 2 — GitHub
1. Créez un dépôt GitHub et transférez les fichiers à la racine du dépôt (`index.html` doit être à la racine).
2. Cloudflare Pages → Connect to Git → sélectionnez le dépôt.
3. Framework preset: **None**. Build command: **vide**. Output directory: **/** (root).
4. Déployez et utilisez `https://votre-projet.pages.dev/catalogue/`.

## QR code
Dès que l'URL publique fonctionne, générez un QR code pointant vers l'URL finale `/catalogue/`. Il est impossible de créer un QR définitif avant d'avoir votre vraie adresse `pages.dev` ou domaine personnalisé.

## Modifier les prix
Changez les montants dans `catalogue/index.html`, puis redéployez. Si vous voulez que le PDF affiche les mêmes prix modifiés, remplacez aussi `assets/catalogue-emballages.pdf`.

Le chemin `/catalogue/` reste stable d'une mise à jour à l'autre. Tant que ce lien ne change pas, le même QR code continue à fonctionner.
