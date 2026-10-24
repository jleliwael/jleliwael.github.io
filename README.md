# Portfolio — Wael Jleli

Site statique (HTML/CSS/JS, aucune dépendance à installer).

```
portfolio-wael/
├── index.html              ← la page
└── assets/
    ├── photo.jpg           ← photo de profil
    └── CV_Wael_Jleli.pdf   ← CV téléchargeable depuis le site
```

## Tester en local
Ouvre `index.html` dans ton navigateur, ou lance un petit serveur :
```bash
cd portfolio-wael
python3 -m http.server 8000   # puis http://localhost:8000
```

## Option 1 — GitHub Pages (recommandé, URL : https://jleliwael.github.io)
1. Sur GitHub, crée un dépôt nommé exactement **jleliwael.github.io** (public).
2. Envoie les fichiers :
   ```bash
   cd portfolio-wael
   git init
   git add .
   git commit -m "Portfolio"
   git branch -M main
   git remote add origin https://github.com/jleliwael/jleliwael.github.io.git
   git push -u origin main
   ```
3. Dans le dépôt : **Settings → Pages → Source : Deploy from a branch → main / (root)** → Save.
4. Après 1 à 2 minutes, le site est en ligne sur **https://jleliwael.github.io**.

## Option 2 — Netlify (le plus rapide, sans Git)
1. Va sur https://app.netlify.com/drop
2. Glisse-dépose le dossier `portfolio-wael` entier.
3. Tu obtiens une URL publique immédiatement (renommable dans *Site settings → Change site name*).

## Option 3 — Vercel
```bash
npm i -g vercel
cd portfolio-wael
vercel --prod
```

## Mettre à jour
- Texte : modifie directement `index.html`.
- Photo / CV : remplace les fichiers dans `assets/` en gardant les mêmes noms.
- Puis `git add . && git commit -m "Mise à jour" && git push` (GitHub Pages se met à jour tout seul).

## Astuce
Ajoute le lien du site sur ton CV, ton profil LinkedIn et dans la description de ton profil GitHub.
