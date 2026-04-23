# SEO-rapport dkf.be — De Content Studio

Onafhankelijk Ahrefs-gestuurd SEO-rapport voor dkf.be.
Snapshot 23 april 2026, markt BE (NL).

Statische single-page HTML, geen build-stap, geen dependencies. Klaar voor directe deploy via Vercel.

## 📂 Inhoud

```
.
├── index.html      # Het volledige rapport
└── README.md       # Dit bestand
```

## 🚀 Deploy via GitHub + Vercel

### Eénmalig: nieuwe GitHub repo

```bash
cd dkf-rapport
git init
git add .
git commit -m "Initial: dkf.be SEO-rapport v1.0"
git branch -M main
git remote add origin git@github.com:<jouw-username>/dkf-rapport.git
git push -u origin main
```

### Eénmalig: koppelen aan Vercel

1. Ga naar [vercel.com/new](https://vercel.com/new)
2. Importeer de GitHub repo `dkf-rapport`
3. Framework Preset: **Other** (geen build nodig)
4. Build Command: leeg laten
5. Output Directory: leeg laten (root)
6. Klik **Deploy**

Vercel detecteert automatisch dat het een statische site is en serveert `index.html` op de root.

### Resultaat

- Productie-URL: `https://<projectnaam>.vercel.app`
- Optioneel custom domain via Vercel → Settings → Domains
  (bv. `rapport.decontentstudio.be` of `dkf.decontentstudio.be`)

### Updates

```bash
# wijziging maken in index.html
git add index.html
git commit -m "Update: ..."
git push
```

Vercel deployt automatisch bij elke push naar `main`.

## 🔒 Toegang beperken (optioneel)

Het rapport bevat `<meta name="robots" content="noindex,nofollow">` zodat het niet in zoekmachines verschijnt.

Voor extra bescherming: in Vercel → Settings → Deployment Protection → **Vercel Authentication** of **Password Protection** activeren. Vereist Pro-plan voor password protection op een hobby-project.

## 🎨 Branding

Visueel design in DCS-stijl:
- Editoriale typografie (Fraunces voor display, Manrope voor body, JetBrains Mono voor cijfers)
- Cream + ink + warm accent palet
- Magazine-spread compositie
- Print-friendly stylesheet ingebouwd (Cmd/Ctrl + P)

Alle stijlen zijn inline in `index.html` — geen extra CSS-bestanden.

## 📝 Versies

| Versie | Datum | Wijzigingen |
|---|---|---|
| 1.0 | 23.04.2026 | Eerste publicatie |

---

**Opgesteld door De Content Studio** · no-nonsense storytelling
