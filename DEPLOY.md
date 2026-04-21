# Deploy til backstage.iconhair.dk — Trin-for-trin guide

## Hvad du deployer
En præsentationsside der viser Icon Backstage-appen inde i en iPhone-mockup på desktop, og direkte i fuld skærm på mobil. Password: **Anker**

---

## Trin 1 — Opret Vercel-konto (gratis)
1. Gå til [vercel.com](https://vercel.com) og opret en gratis konto (brug din email)

---

## Trin 2 — Upload filerne til Vercel
**Nemmeste metode — drag & drop:**
1. Gå til [vercel.com/new](https://vercel.com/new)
2. Klik **"Browse"** eller træk mappen `icon-backstage-presentation` ind
3. Vercel registrerer automatisk at det er en statisk side
4. Klik **Deploy** — tager ~10 sekunder

---

## Trin 3 — Tilføj dit eget domæne (backstage.iconhair.dk)
1. Gå til dit projekt på Vercel → **Settings** → **Domains**
2. Skriv `backstage.iconhair.dk` og klik **Add**
3. Vercel viser dig en DNS-record (CNAME eller A-record)
4. Log ind hos din DNS-udbyder (typisk dit domæneregistrar, f.eks. One.com, GoDaddy, Cloudflare)
5. Tilføj den DNS-record Vercel viser
6. Vent 5-30 minutter — så er `backstage.iconhair.dk` live!

---

## Trin 4 — Test
- Åbn `backstage.iconhair.dk` i en browser
- Skriv password: **Anker**
- Appen vises i iPhone-ramme på desktop
- På mobil (iPhone/Android) vises appen i fuld skærm

---

## Vigtigt: App-serveren skal køre
Appen inde i iPhone-rammen hentes fra Manus-serveren. Denne server kører automatisk når du arbejder i Manus. Til præsentationen: sørg for at have Manus-projektet åbent i en fane.

**Til permanent hosting:** Kontakt Manus support for at få en permanent URL til appen.

---

## Filer i denne mappe
- `index.html` — Præsentationssiden (password-gate + iPhone-mockup)
- `vercel.json` — Vercel-konfiguration
- `DEPLOY.md` — Denne guide
