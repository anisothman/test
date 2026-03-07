# QCM — Fondamentaux des Tests Logiciels (ISTQB)

## 📁 Structure du projet
```
qcm-vercel/
├── api/
│   └── claude.js        ← Fonction serverless (proxy API)
├── public/
│   └── index.html       ← Interface du QCM
├── vercel.json          ← Configuration Vercel
├── package.json
└── README.md
```

---

## 🚀 Déploiement en 5 étapes

### Étape 1 — Créer un compte GitHub
👉 https://github.com → Sign up

### Étape 2 — Uploader sur GitHub
1. Cliquer **New repository**
2. Nom : `qcm-test-logiciel`
3. Cliquer **Create repository**
4. Cliquer **Add file** → **Upload files**
5. Uploader TOUS les fichiers en respectant la structure des dossiers
6. Cliquer **Commit changes**

### Étape 3 — Créer un compte Vercel
👉 https://vercel.com → Sign up with GitHub

### Étape 4 — Déployer sur Vercel
1. Cliquer **Add New Project**
2. Sélectionner votre repo `qcm-test-logiciel`
3. Cliquer **Deploy**

### Étape 5 — Ajouter la clé API (IMPORTANT !)
1. Dans Vercel → votre projet → **Settings**
2. Aller dans **Environment Variables**
3. Ajouter :
   - **Name** : `ANTHROPIC_API_KEY`
   - **Value** : `sk-ant-votre-vraie-cle-ici`
4. Cliquer **Save**
5. Aller dans **Deployments** → cliquer **Redeploy**

✅ Votre QCM est maintenant en ligne sur `https://votre-projet.vercel.app`

---

## 🔑 Obtenir une clé API Anthropic
👉 https://console.anthropic.com
- Créer un compte
- Aller dans **API Keys**
- Cliquer **Create Key**
- Copier la clé (commence par `sk-ant-...`)

---

## 🔒 Sécurité
- La clé API est stockée dans les variables d'environnement Vercel
- Elle n'est JAMAIS visible dans le code HTML ou GitHub
- Chaque utilisateur du site génère ses propres questions via votre clé



