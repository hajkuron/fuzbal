# Firebase Configuration Setup

## 🔒 Using GitHub Secrets (Recommended for Production)

Your Firebase configuration is stored as GitHub Secrets and injected during deployment.

### Step 1: Add Secrets to GitHub

1. Go to your repository: https://github.com/hajkuron/fuzbal
2. Click **Settings** → **Secrets and variables** → **Actions**
3. Click **New repository secret** and add each of these:

   - `FIREBASE_API_KEY`: `AIzaSyDNtYSNhA7GGqOZZCW7DCRfimEQkv3NA2A`
   - `FIREBASE_AUTH_DOMAIN`: `fuzbal-b5439.firebaseapp.com`
   - `FIREBASE_DATABASE_URL`: `https://fuzbal-b5439-default-rtdb.europe-west1.firebasedatabase.app`
   - `FIREBASE_PROJECT_ID`: `fuzbal-b5439`
   - `FIREBASE_STORAGE_BUCKET`: `fuzbal-b5439.firebasestorage.app`
   - `FIREBASE_MESSAGING_SENDER_ID`: `87140388690`
   - `FIREBASE_APP_ID`: `1:87140388690:web:1976fe3d2551203417b48b`

### Step 2: Enable GitHub Actions

The workflow will automatically create `config.js` from secrets when you push to the repo.

---

## 🛠️ Local Development Setup

For local development, create `config.js` from the template:

1. Copy the example file:
   ```bash
   cp config.js.example config.js
   ```

2. Edit `config.js` and add your Firebase credentials

3. `config.js` is gitignored and won't be committed to the repo

---

## 📝 Important Notes

- **`config.js`** is gitignored - it contains your secrets
- **`config.js.example`** is in the repo as a template
- GitHub Actions will create `config.js` from secrets during deployment
- Never commit `config.js` to the repository!

