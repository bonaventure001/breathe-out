# Breathe-Out 🌿

> Your health companion for crypto users. Not financial advice — just a friend who cares.

## What it does

Breathe-Out is an AI-powered emotional health chatbot built for crypto users. It detects stress, burnout, FOMO, and overtrading patterns, and offers calm, grounded guidance — without ever giving financial or medical advice.

---

## 🚀 Deploy in 5 minutes (no coding needed)

### Step 1 — Put the code on GitHub

1. Go to [github.com](https://github.com) and create a free account
2. Click the **+** icon → **New repository**
3. Name it `breathe-out`, set it to **Public**, click **Create repository**
4. Click **uploading an existing file** on the next screen
5. Drag and drop ALL the files from this folder into the upload area
6. Click **Commit changes**

---

### Step 2 — Connect to Netlify

1. Go to [netlify.com](https://netlify.com) and sign up free (use your GitHub account)
2. Click **Add new site** → **Import an existing project**
3. Choose **GitHub** → find and select your `breathe-out` repository
4. Leave all settings as default — Netlify will auto-detect the `netlify.toml` config
5. Click **Deploy site**

Your live URL will appear in about 30 seconds — something like `https://breathe-out-abc123.netlify.app`

You can change this to a custom name under **Site settings → Domain management**.

---

### Step 3 — Add your GitHub Actions secrets (for auto-deploy on every save)

This makes it so every time you edit a file on GitHub, your live site updates automatically.

1. In Netlify: Go to **Site settings → API** → copy your **Site ID**
2. In Netlify: Go to **User settings → Applications → Personal access tokens** → create a new token → copy it
3. In GitHub: Go to your `breathe-out` repo → **Settings → Secrets and variables → Actions**
4. Add two secrets:
   - Name: `NETLIFY_SITE_ID` → paste your Site ID
   - Name: `NETLIFY_AUTH_TOKEN` → paste your Netlify token
5. Done — every push to `main` now auto-deploys ✅

---

## ✏️ How to make edits after launch

You never need to touch code. Just:

1. Go to your repo on GitHub
2. Click `index.html`
3. Click the pencil ✏️ icon to edit
4. Make your change (e.g. update a label, change a colour, edit a message)
5. Click **Commit changes**
6. Netlify detects the change and redeploys automatically in ~30 seconds

---

## 📁 File structure

```
breathe-out/
├── index.html              ← The entire app (one file)
├── netlify.toml            ← Netlify deployment config
├── .gitignore              ← Files Git should ignore
├── .github/
│   └── workflows/
│       └── deploy.yml      ← Auto-deploy on every push
└── README.md               ← This file
```

---

## 🔑 API Key

Breathe-Out uses the Anthropic Claude API to power the chatbot. Users enter their own API key in the app — it is stored only in their browser and never sent to any server other than Anthropic directly.

Get a free API key at: [console.anthropic.com](https://console.anthropic.com)

---

## ⚠️ Disclaimer

Breathe-Out is not a medical tool, therapy service, or financial advisor. It is a wellness companion. Always encourage users to seek professional help for serious mental or physical health concerns.

---

Built with care. For the degens who need to breathe-out. 🌿
