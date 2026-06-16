# UFAICE — AGI Service as a Software

**Erez Glik** | Integration Consultant Engineer  
DevOps · Cloud · SecOps · BigFix · SRE · GenAI / AGI

---

## Live URLs

| Environment | URL |
|---|---|
| Custom domain | https://ufaice.com/ |
| Cloudflare Pages | https://ufaice.pages.dev/ |
| AQ (AI Queue) | https://aq-ufaceit.lovable.app |
| GitHub source | https://github.com/eg185044/AQ |

---

## Cloudflare Pages build settings

```
Framework preset:       None
Build command:          (leave blank)
Build output directory: /
Root directory:         /
Production branch:      main
```

These settings are configured in:  
**Cloudflare Dashboard → Workers & Pages → ufaice → Settings → Builds & deployments**

---

## Git deploy workflow

Every push to `main` triggers an automatic Cloudflare Pages deployment.

```powershell
git add .
git commit -m "Update UFAICE PWA"
git push origin main
```

Check deployment status:  
**Cloudflare Dashboard → Workers & Pages → ufaice → Deployments**

---

## Local development

### Python (simplest)
```powershell
cd $HOME\Dev\AQ
python -m http.server 8080
# Open: http://localhost:8080
```

### VS Code Live Server
Install the **Live Server** extension, right-click `index.html` → **Open with Live Server**.

---

## Project structure

```
AQ/
├── index.html            # Main PWA page
├── style.css             # Dark DevOps-style theme
├── manifest.webmanifest  # PWA manifest
├── service-worker.js     # Offline shell cache
├── robots.txt            # Search engine rules
└── README.md             # This file
```

---

## Contact

- Email: [GlikErez@ufaice.Com](mailto:GlikErez@ufaice.Com)
- LinkedIn: [linkedin.com/in/ErezGlik](https://linkedin.com/in/ErezGlik)
- GitHub: [github.com/eg185044/DevOps](https://github.com/eg185044/DevOps)
