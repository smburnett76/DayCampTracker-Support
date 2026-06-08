# Day Camp Tracker — Support

Public support site and privacy policy for the **Day Camp Tracker** iOS app ([DayCampTracker](https://github.com/smburnett76/DayCampTracker)).

## GitHub Pages

- **Site:** https://smburnett76.github.io/DayCampTracker-Support/
- **Privacy policy (App Store Connect):** https://smburnett76.github.io/DayCampTracker-Support/privacy-policy

Enable Pages: repo **Settings → Pages →** source **Deploy from branch** → **main** → **/ (root)**.

## Contact

**sbapp_support@icloud.com**

## Files

| File | Purpose |
|------|---------|
| `index.md` | Support home page |
| `privacy-policy.md` | Privacy policy (linked from App Store Connect) |
| `_config.yml` | Jekyll / Pages config (`baseurl` must match repo name) |

## Sync with the app repo

When you change privacy text in **DayCampTracker** `docs/privacy-policy.md`, copy sections **1–11** (through **Contact us**) into this repo’s `privacy-policy.md`. Keep the YAML front matter here; omit the app-repo dev note at the top and **Section 12** (App Store privacy labels). Use a `mailto:` link for the support email on the published page.
