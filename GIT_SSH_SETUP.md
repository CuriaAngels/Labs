# Git SSH Setup – CuriaAngels/Labs

**Main repo:** https://github.com/CuriaAngels/Labs

Use SSH instead of HTTPS for pushing to this repo.

---

## 1. Generate SSH key

```bash
ssh-keygen -t ed25519 -C "curia.angels.labs@gmail.com" -f ~/.ssh/id_ed25519_curiaangels
```

Press Enter for default passphrase (or set one).

---

## 2. Add key to ssh-agent

```bash
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519_curiaangels
```

---

## 3. Add public key to GitHub

1. Copy your public key:
   ```bash
   cat ~/.ssh/id_ed25519_curiaangels.pub
   ```
2. Go to **https://github.com/settings/keys**
3. Click **New SSH key**
4. Title: `Curia Angels Labs`
5. Paste the key → **Add SSH key**

---

## 4. Test connection

```bash
ssh -T git@github.com
```

You should see: `Hi CuriaAngels! You've successfully authenticated...`

---

## 5. Clone or set remote

**Clone (fresh):**
```bash
git clone git@github.com:CuriaAngels/Labs.git
cd Labs
```

**Change existing remote to SSH:**
```bash
git remote set-url origin git@github.com:CuriaAngels/Labs.git
```

---

## 6. Push privacy policy (when ready)

```bash
# Copy privacy-policy.html to index.html for GitHub Pages
cp privacy-policy.html index.html

git add index.html
git commit -m "Add CardNest privacy policy"
git push -u origin main
```

Then enable GitHub Pages (see `PRIVACY_POLICY_SETUP.md`).
