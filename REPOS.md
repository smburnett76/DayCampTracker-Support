# Two-repo setup

| Repository | Visibility | Purpose |
|------------|------------|---------|
| **CampTrack** | Private | iOS source code, Xcode project, internal spec |
| **CampTrack-Support** | Public | App Store **Privacy Policy URL**, **Support URL**, contact info |

## Publish CampTrack-Support

```bash
cd CampTrack-Support
git init
git add README.md privacy-policy.md .nojekyll
git commit -m "Add support page and privacy policy for App Store"
git branch -M main
git remote add origin https://github.com/YOUR_GITHUB_USERNAME/CampTrack-Support.git
git push -u origin main
```

Enable **GitHub Pages** (Settings → Pages → branch `main`, folder `/`).

## Publish CampTrack (private)

```bash
cd "Camp Track"   # your local app folder name
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_GITHUB_USERNAME/CampTrack.git
git push -u origin main
```

On GitHub, set the **CampTrack** repository to **Private**.

## App Store Connect URLs

Replace `YOUR_GITHUB_USERNAME`:

| Field | URL |
|-------|-----|
| Privacy Policy | `https://YOUR_GITHUB_USERNAME.github.io/CampTrack-Support/privacy-policy` |
| Support URL | `https://YOUR_GITHUB_USERNAME.github.io/CampTrack-Support/` |

When you change the privacy policy, update **`CampTrack-Support/privacy-policy.md`** first, then copy to the private repo’s `docs/privacy-policy.md` if you keep a duplicate for reference.
