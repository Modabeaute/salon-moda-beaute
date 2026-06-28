# 🚀 Guide de mise en ligne — Salon Moda Beauté

Temps estimé : **15 à 20 minutes**

---

## ÉTAPE 1 — Créer un compte GitHub (gratuit)

1. Va sur **https://github.com**
2. Clique sur **"Sign up"**
3. Entre ton email, crée un mot de passe, choisis un nom d'utilisateur
4. Valide ton email

---

## ÉTAPE 2 — Créer un dépôt GitHub avec le site

1. Une fois connecté sur GitHub, clique sur **"New repository"** (bouton vert en haut à droite)
2. Nom du dépôt : `salon-moda-beaute`
3. Laisse tout par défaut, clique **"Create repository"**
4. Maintenant tu vas uploader les fichiers :
   - Clique sur **"uploading an existing file"**
   - Glisse-dépose **tous les fichiers du ZIP** que tu as téléchargé (extrait le ZIP d'abord)
   - ⚠️ Important : uploade les fichiers **ET** les dossiers (`src/`, `public/`)
   - Clique **"Commit changes"**

---

## ÉTAPE 3 — Créer un compte Netlify (gratuit)

1. Va sur **https://netlify.com**
2. Clique **"Sign up"**
3. Choisis **"Sign up with GitHub"** (c'est le plus simple)
4. Autorise Netlify à accéder à GitHub

---

## ÉTAPE 4 — Connecter le site à Netlify

1. Dans Netlify, clique **"Add new site"** → **"Import an existing project"**
2. Clique **"GitHub"**
3. Sélectionne le dépôt `salon-moda-beaute`
4. Les paramètres de build sont déjà configurés (fichier `netlify.toml`) — laisse tout par défaut
5. Clique **"Deploy site"**
6. Attends 1-2 minutes ⏳
7. Ton site est en ligne ! Netlify te donne une URL du type : `random-name-123.netlify.app`

---

## ÉTAPE 5 — Acheter et connecter ton domaine (salonmodabeaute.fr)

### Acheter le domaine
- Va sur **https://www.ionos.fr** ou **https://www.ovhcloud.com/fr/**
- Cherche `salonmodabeaute.fr` (environ 5-10€/an)
- Achète-le

### Connecter le domaine à Netlify
1. Dans Netlify → ton site → **"Domain settings"**
2. Clique **"Add custom domain"**
3. Entre `salonmodabeaute.fr`
4. Netlify te donne des **DNS records** à configurer chez ton registraire (OVH ou IONOS)
5. Dans ton espace OVH/IONOS → DNS → ajoute les records donnés par Netlify
6. Attends 24-48h pour la propagation DNS
7. ✅ Ton site sera accessible sur `salonmodabeaute.fr`

---

## ℹ️ Informations importantes

### Où sont stockées les données ?
Les données (produits, photos, réservations, avis) sont sauvegardées dans le navigateur (**localStorage**).  
**Pour l'admin** : utilise toujours le même appareil (ton téléphone) pour gérer le site.  
Si tu changes d'appareil, tes données admin ne seront pas là — garde une sauvegarde des URLs de tes photos.

### Mot de passe admin
Email : **Salonmodabeaute@gmail.com**  
Mot de passe : **Moda123#**  
(pour changer → modifie les lignes `ADMIN_EMAIL` et `ADMIN_PASSWORD` dans `src/App.jsx`)

### Mises à jour du site
Si tu veux modifier quelque chose dans le code :
1. Modifie le fichier dans GitHub (bouton crayon ✏️)
2. Netlify redéploie automatiquement en 1-2 minutes

### Support
Pour toute aide ou modification du site, reviens sur Claude.ai !

---

## 🆘 En cas de problème

- **Le site ne se charge pas** → vérifie que le build Netlify est passé (onglet "Deploys")
- **L'admin ne fonctionne pas** → vide le cache du navigateur (Ctrl+Shift+R)
- **Les photos ne s'affichent pas** → elles sont liées à l'appareil, il faut les réajouter depuis l'admin

---

Bonne mise en ligne ! 💛🖤
