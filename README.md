# 👨‍💻 charlymedina.fr

Code source de mon site personnel, en ligne sur **[charlymedina.fr](https://charlymedina.fr)**.

Une page de présentation unique : photo, nom, ville (Tours) et liens vers mes réseaux.

---

## 🔗 Contenu

Liens vers mes profils :
[Instagram](https://www.instagram.com/charlymedina.fr/) ·
[Strava](https://www.strava.com/athletes/charlymedina) ·
[GitHub](https://github.com/charlymedina) ·
[LinkedIn](https://www.linkedin.com/in/charlymedina/)

## 🛠️ Technique

- **Site statique** : un seul `index.html` avec CSS intégré, sans JavaScript ni build.
- **Images** : WebP, sans métadonnées EXIF/GPS.
- **Hébergement** : Cloudflare Pages (projet `charlymedina`).
- **Statistiques** : Cloudflare Web Analytics (sans cookie).
- **Déploiement** : GitHub Action (`.github/workflows/deploy.yml`) à chaque push sur `main`.

## 📁 Structure

```
├── public/                    # Contenu publié
│   ├── index.html             # La page du site
│   ├── images/                # lac (fond), profil, og.jpg (aperçu de partage)
│   └── favicon.*, apple-touch-icon.png, android-chrome-*, site.webmanifest
└── .github/workflows/deploy.yml
```

## ✏️ Modifier le site

1. Modifier `public/index.html` ou remplacer les images dans `public/images/`.
2. Commit + push sur `main` : l'action GitHub republie le site sur Cloudflare en une minute environ.
