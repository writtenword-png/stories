# Mes Nouvelles — Guide de mise en ligne

Votre site se compose de deux fichiers seulement :

```
index.html     ← la page que voient vos lecteurs
stories.json   ← votre "backend" : ajoutez vos nouvelles ici
```

---

## Ajouter ou modifier une nouvelle

Ouvrez `stories.json` et suivez ce format :

```json
[
  {
    "id": "1",
    "title": "Le titre de votre nouvelle",
    "date": "2025-06-15",
    "body": "Premier paragraphe de votre nouvelle.\n\nDeuxième paragraphe (séparé par une ligne vide).\n\nTroisième paragraphe, etc."
  },
  {
    "id": "2",
    "title": "Une autre nouvelle",
    "date": "2025-07-01",
    "body": "Texte de la deuxième nouvelle..."
  }
]
```

> **Important** : séparez les paragraphes avec `\n\n` dans le JSON.  
> La `date` est optionnelle (format AAAA-MM-JJ).

---

## Mettre en ligne gratuitement sur GitHub Pages

1. Créez un compte sur [github.com](https://github.com) si vous n'en avez pas
2. Créez un nouveau dépôt public (ex: `mes-nouvelles`)
3. Glissez-déposez `index.html` et `stories.json` dans le dépôt
4. Allez dans **Settings → Pages → Source : Deploy from a branch → main / root**
5. Votre site sera disponible à l'adresse :  
   `https://VOTRE_PSEUDO.github.io/mes-nouvelles/`

Pour mettre à jour vos nouvelles : modifiez `stories.json` sur GitHub et validez. Le site se met à jour en 1-2 minutes.

---

## Autres options d'hébergement

| Service | Gratuit | Facilité |
|---|---|---|
| GitHub Pages | ✅ | ★★★ |
| Netlify Drop | ✅ | ★★★★ (glisser-déposer) |
| Vercel | ✅ | ★★★ |

Pour Netlify : allez sur [app.netlify.com/drop](https://app.netlify.com/drop) et glissez le dossier entier. Vous obtenez un lien immédiatement.
