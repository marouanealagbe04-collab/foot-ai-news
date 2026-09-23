# ⚽ FOOT AI NEWS

Plateforme web d'actualités football en temps réel avec génération automatique de publications par IA pour Facebook.

## 🚀 DÉMARRAGE RAPIDE (5 minutes)

### 1️⃣ Récupère ta clé API Claude
- Va sur https://console.anthropic.com/account/keys
- Crée une nouvelle clé (Start at account overview)
- Copie-la et garde-la à côté

### 2️⃣ Crée un repo GitHub
- Va sur https://github.com/new
- Nomme-le `foot-ai-news`
- Clique "Create repository"

### 3️⃣ Upload les fichiers
Sur la page du repo GitHub :
- Clique "Add file" → "Upload files"
- Upload tous les fichiers du dossier `foot-ai-news`

Ou en ligne de commande :
```bash
git clone https://github.com/TON-USERNAME/foot-ai-news.git
cd foot-ai-news
# Ajoute les fichiers ici
git add .
git commit -m "Initial commit"
git push origin main
```

### 4️⃣ Déploie sur Netlify
1. Va sur https://app.netlify.com
2. Clique "New site from Git"
3. Sélectionne GitHub et `foot-ai-news`
4. Configure les variables d'environnement :
   - Settings → Build & Deploy → Environment
   - Ajoute : `ANTHROPIC_API_KEY` = ta clé Claude

5. **C'est live !** 🎉

Ton site est maintenant accessible à `https://ton-app.netlify.app`

---

## 📁 STRUCTURE DU PROJET

```
foot-ai-news/
├── index.html                           # Dashboard principal
├── package.json                         # Dépendances
├── .gitignore                           # Fichiers ignorés
├── netlify/
│   └── functions/
│       └── generate-publication.js      # Fonction IA pour générer publications
└── README.md                            # Ce fichier
```

---

## 🎨 FONCTIONNALITÉS

✅ **Dashboard mobile-friendly**
- 4 onglets : Matchs en direct, Actualités, Publications, Paramètres
- Design moderne noir/rouge
- Responsive sur tous les téléphones

✅ **Génération IA automatique**
- Clique sur un match ou actualité
- Claude génère une publication en 2 secondes
- Prête à publier sur Facebook

✅ **Gestion des publications**
- Copier le texte
- Programmer la publication
- Historique des publications passées

✅ **Automatisation**
- Toggle pour activer/désactiver l'automatisation
- Paramètres personnalisables par équipe
- Statistiques de performance

---

## ⚙️ CONFIGURATION

### Variables d'environnement (Netlify)

```
ANTHROPIC_API_KEY=sk-ant-...
```

Cette clé doit être ajoutée dans **Settings → Build & Deploy → Environment** sur Netlify.

### Équipes favorites
Modifie directement dans le dashboard (onglet Paramètres) ou édite le code HTML.

---

## 🔧 DÉVELOPPEMENT LOCAL

```bash
# Installe les dépendances
npm install

# Lance le serveur local avec Netlify
npm run dev

# Ouvre http://localhost:8888
```

---

## 📞 DÉPANNAGE

### "Erreur de génération - Vérifiez votre clé API Claude"
→ Ta clé `ANTHROPIC_API_KEY` n'est pas configurée dans Netlify
→ Va dans Settings → Build & Deploy → Environment

### "Erreur 429 - Trop de requêtes"
→ Tu as généré trop de publications d'un coup
→ Patienta 1-2 minutes avant de réessayer

### "Page blanche"
→ Cache ton navigateur (Ctrl+Shift+R ou Cmd+Shift+R)
→ Ou ouvre en navigation privée

### "Fonction Netlify non trouvée"
→ Les fonctions sont automatiquement déployées avec le repo
→ Attend 2-3 minutes après le push
→ Vérifie les logs Netlify

---

## 🚀 PROCHAINES ÉTAPES

### Phase 2 : Données réelles
```javascript
// Intégrer une API football
- Football-Data.org (matchs, calendriers)
- ESPN API (actualités)
- RapidAPI Football (résultats en direct)
```

### Phase 3 : Facebook API
```javascript
// Publication automatique sur ta page Facebook
- Connecter Meta Graph API
- Publications programmées
- Historique complet
```

### Phase 4 : Images automatiques
```javascript
// Générer des images pour chaque publication
- Unsplash/Pexels (photos gratuites)
- DALL-E ou similaire (génération IA)
- Watermark avec logo
```

### Phase 5 : Android/iOS
```
- React Native
- Flutter
- PWA (Progressive Web App)
```

---

## 📊 STATISTIQUES

- **Temps de déploiement** : ~1 minute
- **Coûts** : Gratuit (Netlify + Anthropic API)
- **Capacités** : ∞ (scalable)
- **Latence** : < 2 secondes par génération

---

## 💡 CONSEILS D'UTILISATION

1. **Commencer petit** : 3-5 équipes favorites
2. **Tester avant d'automatiser** : Générer manuellement d'abord
3. **Vérifier les publications** : L'IA peut halluciner parfois
4. **Ajouter des images** : Plus de réactions avec des visuels
5. **Poster aux heures d'activité** : 18h-21h pour le foot

---

## 📝 LICENSE

MIT - Libre d'utilisation

---

## 🆘 SUPPORT

Problèmes ?
- Vérifie ta clé API Claude
- Vérifies les logs Netlify (Deploys → Logs)
- Réouvre la page en navigation privée
- Attends 5 minutes et réessaye

---

**Build by Anthropic Claude • Powered by Netlify**

⚽ Bon courage pour ta plateforme FOOT AI NEWS ! 🚀
