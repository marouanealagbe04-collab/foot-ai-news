# 🚀 GUIDE DE DÉPLOIEMENT FOOT AI NEWS

**Durée totale : 10 minutes**

---

## ✅ AVANT DE COMMENCER

Tu auras besoin de :
- Un compte GitHub (gratuit)
- Un compte Netlify (gratuit, via GitHub)
- Ta clé API Claude (de console.anthropic.com)

---

## 📋 ÉTAPE 1 : Préparer ta clé Claude (2 min)

1. Ouvre **https://console.anthropic.com/account/keys**
2. Clique "Create key"
3. Nomme-la `foot-ai-news`
4. **Copie la clé complète** (elle commence par `sk-ant-`)
5. Garde-la dans un bloc-notes pour l'étape 4

⚠️ **IMPORTANT** : Ne partage JAMAIS cette clé avec personne !

---

## 🔗 ÉTAPE 2 : Créer un repo GitHub (2 min)

1. Ouvre **https://github.com/new**
2. Remplis :
   - **Repository name** : `foot-ai-news`
   - **Description** : Plateforme d'actualités football avec IA
   - **Public** : ✓ Coché
3. Clique "Create repository"
4. **Reste sur cette page**, on revient tout de suite

---

## 📤 ÉTAPE 3 : Upload les fichiers (3 min)

Sur la page GitHub du repo que tu viens de créer :

1. Clique le bouton vert **"Code"**
2. En bas, clique **"Upload files"**
3. **Uploads ces 5 fichiers** (en copiant leur contenu) :

   **Option A : Upload directement**
   - Va dans les fichiers que tu as téléchargés
   - Drag & drop tous les fichiers vers GitHub
   
   **Option B : Copier-coller**
   - Pour chaque fichier, clique "+ Add file" → "Create new file"
   - Nomme-le correctement
   - Copie le contenu
   - Clique "Commit changes"

**Fichiers à uploader :**
```
- index.html
- package.json
- .gitignore
- netlify.toml
- README.md
- netlify/functions/generate-publication.js
```

⚠️ **Pour la fonction** : 
- Crée d'abord le dossier `netlify/`
- Puis le sous-dossier `functions/`
- Puis upload `generate-publication.js` dedans

---

## 🌐 ÉTAPE 4 : Déployer sur Netlify (3 min)

1. Ouvre **https://app.netlify.com**
2. Clique "Sign up" → "Continue with GitHub"
3. Valide la connexion GitHub
4. Une fois connecté, clique **"New site from Git"**
5. Sélectionne **GitHub**
6. Trouve et clique sur **`foot-ai-news`**
7. Laisse les paramètres par défaut et clique **"Deploy site"**

**Attends 2-3 minutes** (tu verras "Deploying site...")

---

## 🔑 ÉTAPE 5 : Ajouter ta clé API (2 min)

Quand le déploiement est terminé :

1. Clique l'onglet **"Site settings"**
2. À gauche, clique **"Build & deploy"**
3. Clique **"Environment"**
4. Clique **"Edit variables"**
5. Ajoute une variable :
   - **Key** : `ANTHROPIC_API_KEY`
   - **Value** : `sk-ant-...` (ta clé de l'étape 1)
6. Clique "Save"
7. Retour à "Deploys" → clique le dernier déploiement → **"Redeploy"**

**Attends 1 minute** que le site se redéploie avec la clé.

---

## ✅ ÉTAPE 6 : Vérifier que ça marche (2 min)

1. Va dans l'onglet **"Deploys"**
2. Tu dois voir "Publish" avec un badge vert ✓
3. Clique sur le lien (exemple : `https://foot-ai-news-123.netlify.app`)
4. La plateforme s'ouvre ! 🎉

**Test rapide :**
1. Onglet "EN DIRECT"
2. Clique "Générer pub" sur un match
3. **Si ça génère une publication** → ✅ Tout fonctionne !

---

## 🎉 C'EST TERMINÉ !

Ton plateforme FOOT AI NEWS est maintenant **en ligne** et **publique** !

### URL de ta plateforme :
```
https://foot-ai-news-XXXX.netlify.app
```

### Ce que tu peux faire maintenant :
- ✅ Générer des publications avec l'IA
- ✅ Partager le lien avec tes amis
- ✅ Faire des tests avant de publier sur Facebook
- ✅ Modifier le design directement dans le code

---

## 🔄 SI QUELQUE CHOSE NE MARCHE PAS

### "Page blanche"
→ Attends 5 minutes et recharge
→ Ou essaie en mode navigation privée (Ctrl+Maj+P)

### "Erreur de génération"
→ Va dans **Netlify Settings → Build & deploy → Environment**
→ Vérifie que `ANTHROPIC_API_KEY` est bien configurée
→ Redéploie le site

### "Site not found"
→ Le déploiement n'est peut-être pas fini
→ Va dans **Deploys** sur Netlify
→ Cherche le dernier déploiement avec badge ✓

### "Autre problème"
→ Logs Netlify : Settings → Logs → Function logs
→ Regarde si y'a des erreurs rouges
→ Screenshot et montre-moi !

---

## 📱 UTILISER DEPUIS TON TÉLÉPHONE

1. Accède à `https://foot-ai-news-XXXX.netlify.app`
2. Ajoute aux favoris (bookmark)
3. Ou crée un raccourci sur l'écran d'accueil :
   - Appuie 3 secondes sur le lien
   - "Ajouter à l'écran d'accueil"

---

## 🚀 PROCHAINES ÉTAPES (OPTIONNEL)

Une fois que c'est live :

1. **Ajouter tes vraies équipes** : Édite le code HTML
2. **Intégrer une API football** : Récupère les vrais matchs en direct
3. **Connecter Facebook** : Publie automatiquement sur ta page
4. **Ajouter des images** : Chaque publication avec une image

---

## 💬 BESOIN D'AIDE ?

Envoie-moi :
- Screenshot du problème
- Le lien de ta plateforme
- L'erreur exacte que tu vois

---

**Prêt ? 🚀 Commence par l'ÉTAPE 1 !**
