# École de l'engagement — Site web

Site web officiel de l'**École de l'engagement**, association loi 1901 qui forme gratuitement des citoyennes et citoyens issus des classes populaires à l'engagement politique, syndical et associatif.

## 🚀 Déploiement sur Vercel

Ce projet est un **site statique** prêt à être déployé sur Vercel sans aucune configuration supplémentaire.

### Étapes de déploiement

1. **Pousser le code sur GitHub** (déjà fait : `https://github.com/kevingaga/EcoleEngagement.git`)
2. Aller sur [vercel.com](https://vercel.com) et se connecter avec GitHub
3. Cliquer sur **"Add New..." → "Project"**
4. Sélectionner le repo **`EcoleEngagement`**
5. Vercel détecte automatiquement qu'il s'agit d'un site statique
6. Laisser tous les réglages par défaut :
   - **Framework Preset** : `Other` (ou laisser vide)
   - **Build Command** : *(vide)*
   - **Output Directory** : *(vide)*
   - **Install Command** : *(vide)*
7. Cliquer sur **"Deploy"**

Le site sera accessible en quelques secondes à une URL du type `https://ecole-engagement.vercel.app`.

### Domaine personnalisé

Pour utiliser un domaine comme `ecole-de-lengagement.fr` :

1. Dans le dashboard Vercel du projet → **Settings** → **Domains**
2. Ajouter le domaine
3. Configurer les DNS chez votre registrar selon les instructions affichées

## 📂 Structure du projet

```
.
├── index.html          # Page d'accueil
├── 404.html            # Page d'erreur personnalisée
├── images/             # Photos des promotions
│   ├── promo-portique.jpg
│   ├── promo-paris.jpg
│   └── promo-batiment.jpg
├── vercel.json         # Configuration Vercel (cache, headers de sécurité)
├── robots.txt          # Directives pour les moteurs de recherche
├── sitemap.xml         # Plan du site pour le SEO
├── .gitignore          # Fichiers ignorés par git
└── README.md           # Ce fichier
```

## 🛠️ Développement local

Aucune dépendance, aucune compilation. Pour prévisualiser le site :

### Option 1 — Ouvrir directement
Double-cliquer sur `index.html`.

### Option 2 — Serveur local (recommandé)
```bash
# Avec Python 3
python3 -m http.server 8000

# Ou avec Node.js
npx serve .
```

Puis ouvrir `http://localhost:8000`.

## ✏️ Personnalisation

### Lien du don (Google Doc)
Dans `index.html`, chercher la ligne suivante et remplacer l'URL :

```html
<a href="https://docs.google.com/" target="_blank" rel="noopener" class="don-cta">
  Faire un don maintenant →
</a>
```

### Liens du footer
Dans `index.html`, section `<footer>` :
- Lien Facebook (déjà présent)
- Liens Twitter / X et Instagram (à compléter)
- Email de contact : `contact@ecole-de-lengagement.fr`

### Ajouter des photos de promotions
1. Ajouter les images dans le dossier `images/`
2. Dans `index.html`, section `<section class="promos">`, dupliquer un bloc `<div class="promo-card">`

## 🎨 Identité visuelle

- **Police titre** : Fraunces (serif éditorial)
- **Police texte** : Inter Tight
- **Couleurs** :
  - Rouge militant : `#B8232A`
  - Crème : `#F4EFE6`
  - Noir doux : `#1A1411`
  - Or accent : `#C8A24A`

## 📝 Mises à jour

Toute modification poussée sur la branche `main` du repo GitHub déclenchera un redéploiement automatique sur Vercel.

```bash
git add .
git commit -m "Mise à jour du contenu"
git push origin main
```

## 📄 Licence

© 2026 École de l'engagement — Tous droits réservés.
