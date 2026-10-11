# Rankr : mise en ligne gratuite

Ce dossier contient le site prêt à publier :

- `index.html` : tout le site (une seule page)
- `manifest.webmanifest`, `icon-192.png`, `icon-512.png`, `sw.js` : permettent d'installer Rankr comme une application sur le téléphone
- `.nojekyll` : fichier vide utile pour GitHub Pages

## Option 1 : GitHub Pages (recommandée, gratuite)

1. Crée un compte gratuit sur https://github.com
2. Clique sur **New repository**. Nom conseillé : `rankr`. Choisis **Public**, puis **Create repository**.
3. Sur la page du dépôt, clique sur **uploading an existing file**.
4. Dézippe ce dossier, puis glisse **tous les fichiers** dedans (y compris `.nojekyll` si ton système l'affiche). Clique sur **Commit changes**.
5. Va dans **Settings > Pages**. Dans « Build and deployment », choisis **Deploy from a branch**, la branche **main** et le dossier **/ (root)**, puis **Save**.
6. Attends 1 à 2 minutes. L'adresse apparaît en haut de la page Pages :
   `https://TON-PSEUDO.github.io/rankr/`

## Option 2 : Cloudflare Pages (bande passante illimitée)

1. Crée un compte gratuit sur https://dash.cloudflare.com
2. Va dans **Workers & Pages**, puis crée un projet Pages avec **Upload assets** (téléversement direct).
3. Donne un nom (par exemple `rankr`), glisse le dossier dézippé et valide.
4. Ton site est disponible à `https://rankr.pages.dev` (l'interface de Cloudflare change parfois : les noms des menus peuvent différer).

## Après la mise en ligne : à vérifier

- Ouvre l'adresse sur ton téléphone et sur ton ordinateur.
- Crée un compte, recharge la page : tu dois rester connecté.
- Sur téléphone : menu du navigateur > **Ajouter à l'écran d'accueil** (ou **Installer l'application**).
- Teste le bouton « Trouver un terrain » : en ligne et avec la position autorisée, la carte tente de charger les vrais terrains (OpenStreetMap).

## Mettre à jour le site plus tard

Remplace le fichier `index.html` dans ton dépôt (**Add file > Upload files**, même nom) puis valide. Le site se met à jour en 1 à 2 minutes. Si tu ne vois pas le changement, recharge la page deux fois.

## À savoir

- Hébergement et adresse : gratuits. Un nom de domaine à toi (`rankr.fr`) est payant, mais se branche ensuite gratuitement.
- Les comptes et les données sont enregistrés **dans le navigateur de chaque joueur**, pas sur un serveur. Deux joueurs ne partagent donc pas encore la même ligue. Pour cela, l'étape suivante est une base de données partagée (par exemple Supabase).
- Avec GitHub Pages gratuit, le code du site est public. Ne mets jamais de mot de passe ou de clé secrète dans `index.html`.
