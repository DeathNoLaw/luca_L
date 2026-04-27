# Lucas L. — Site vitrine one-page

Site statique pour Lucas L., créateur de serveurs Discord.
Stack : **HTML + CSS purs**. Pas de build, pas de framework, pas de JS, pas de tracking.

## Structure

```
index.html   # contenu et structure sémantique
style.css    # design sombre, responsive, mobile-first
```

## Démarrage local

Ouvre simplement `index.html` dans un navigateur, ou sers le dossier :

```bash
python3 -m http.server 8080
# puis http://localhost:8080
```

## Déploiement

N'importe quel hébergeur statique fait l'affaire :

- **Netlify / Vercel / Cloudflare Pages** : drag & drop du dossier ou connexion au dépôt Git
- **GitHub Pages** : pousser sur `main`, activer Pages dans les paramètres
- **OVH / hébergement classique** : uploader `index.html` et `style.css` à la racine

## Personnalisation rapide

- **Contact** : remplacer `mailto:contact@Lucasl.fr` et le lien Discord dans `index.html`
- **Couleurs** : variables CSS dans `:root` au début de `style.css`
- **Typographie** : Inter via Google Fonts (peut être remplacée par une police système pour plus de perf)

## Performance / éco-conception

- Aucun JS, aucune dépendance lourde
- Icônes en SVG inline (pas de fonte d'icônes)
- Police chargée avec `display=swap` et `preconnect`
- Aucune image externe, aucun cookie, aucun tracker
