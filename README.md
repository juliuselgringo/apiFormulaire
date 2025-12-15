# API Formulaire

Une API statique simple hébergée sur GitHub Pages, exposant des données de formulaire au format JSON.

## 📋 Description

Ce projet fournit un fichier JSON contenant des données de formulaire, accessible via une URL publique sur GitHub Pages. Idéal pour :
- Servir des données statiques sans backend
- Tester des appels API avec des données réelles
- Prototyper des applications frontend

## 🚀 Accès

Une fois GitHub Pages activé, les données sont disponibles à :
```
https://<ton-username>.github.io/apiFormulaire/formData.json
```

## 📦 Structure du projet

```
apiFormulaire/
├── README.md              # Ce fichier
├── formData.json          # Données du formulaire (JSON)
└── .git/                  # Dépôt Git
```

## 📖 Utilisation

### Avec JavaScript (fetch)

```javascript
fetch('https://<ton-username>.github.io/apiFormulaire/formData.json')
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.error('Erreur :', error));
```

### Avec curl

```bash
curl https://<ton-username>.github.io/apiFormulaire/formData.json
```

## ✏️ Modifier les données

1. Édite le fichier [formData.json](formData.json)
2. Effectue un commit :
   ```bash
   git add formData.json
   git commit -m "Mise à jour des données du formulaire"
   ```
3. Push vers GitHub :
   ```bash
   git push origin main
   ```
4. Les changements sont live après quelques secondes

## ⚙️ Configuration de GitHub Pages

1. Va dans **Settings** du dépôt
2. Sélectionne **Pages** dans le menu latéral
3. Configure :
   - **Source** : Deploy from a branch
   - **Branch** : `main` (ou `gh-pages`)
   - **Folder** : `/ (root)`
4. Sauvegarde et attends que le statut passe au vert

## 📝 Notes

- ✅ Données en lecture seule (pas de POST/PUT/DELETE)
- ✅ Hébergement gratuit et illimité
- ✅ HTTPS automatique
- ⏱️ Latence mineure lors du redeploy (quelques secondes)

## 📄 Licence

MIT (ou à adapter selon tes besoins)

---

Créé avec GitHub Pages | Dernier déploiement : décembre 2025
