# NAAN HOOD · Démo TK Digital

Site de démonstration single-page pour le portfolio TK Digital.
Marque fictive de street food.

## Structure des fichiers

```
naan-hood/
├── index.html        ← Le site complet (HTML + CSS + JS inline)
├── README.md
└── assets/
    ├── hero.jpg      ← Bannière hero
    ├── naan_1.png    ← Naan Farmer
    ├── naan_2.png    ← Naan Tenders
    ├── naan_3.png    ← Naan Radikal
    ├── naan_4.png    ← Naan Combo
    ├── naan_5.png    ← Naan Boursin
    └── naan_6.png    ← Naan Merguez
```

## Déploiement GitHub Pages (pas à pas)

### 1. Créer le repo

Sur github.com, connecté avec ton compte `tar5950` :

- Clique sur le `+` en haut à droite → **New repository**
- **Repository name** : `naan-hood`
- Coche **Public** (obligatoire pour GitHub Pages gratuit)
- Ne coche PAS "Add a README file" (on en a déjà un)
- Clique **Create repository**

### 2. Upload les fichiers

Sur la page du repo vide qui s'ouvre :

- Clique sur **"uploading an existing file"** (lien dans le bloc gris central)
- Drag and drop **les deux** : le fichier `index.html` ET le dossier `assets` entier
  - Si le drag du dossier ne marche pas, drag les fichiers un par un en gardant `assets/naan_1.png` pour préserver l'arborescence
- Tout en bas, dans "Commit changes", laisse le message par défaut
- Clique le bouton vert **Commit changes**

### 3. Activer GitHub Pages

- Dans le repo, va dans **Settings** (onglet tout en haut à droite)
- Dans le menu de gauche, clique **Pages**
- Section **"Build and deployment"** :
  - **Source** : `Deploy from a branch`
  - **Branch** : `main` · dossier `/ (root)`
- Clique **Save**

### 4. URL du site en ligne

GitHub met 1 à 2 minutes pour publier. Ton URL sera :

```
https://tar5950.github.io/naan-hood/
```

Si tu rafraîchis la page Settings → Pages, tu verras un bandeau vert "Your site is live at..." quand c'est prêt.

## Test en local (sans GitHub)

Dézippe le projet, double-clique sur `index.html`. Ça s'ouvre dans ton navigateur. Tout fonctionne en local sauf que le lien WhatsApp ouvrira quand même `wa.me/33768789800`.

## Personnalisation rapide

Toute la config est centralisée en haut du `<script>` dans `index.html` :

```javascript
const CONFIG = {
    whatsapp: '33768789800',
    telephone: '07 68 78 98 00',
    adresse: '...',
    ville: 'Douai',
    horaires: 'Lun-Dim · 11h-23h',
    instagram: '#',
    tiktok: '#',
};
```

Le menu se modifie dans la constante `MENU` juste en dessous.

## Disclaimer

Marque fictive · Portfolio démo · Aucune commande réelle traitée.

