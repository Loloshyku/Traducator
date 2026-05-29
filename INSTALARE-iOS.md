# Traducător Claude — PWA pentru iPhone / iPad

## Ce este aceasta?

O aplicație web progresivă (PWA) care se instalează pe ecranul de start
al oricărui iPhone sau iPad, funcționând ca o aplicație nativă.

---

## Metoda 1: GitHub Pages (GRATUITĂ, recomandat)

### Pas 1 — Creează un cont GitHub
→ https://github.com → Sign up (gratuit)

### Pas 2 — Creează un repository nou
1. Click „+" → „New repository"
2. Nume: `traducator-claude`
3. Bifează „Add a README file"
4. Click „Create repository"

### Pas 3 — Încarcă fișierele
1. În repository, click „Add file" → „Upload files"
2. Trage TOATE fișierele din acest folder (inclusiv folderul `icons/`)
3. Click „Commit changes"

### Pas 4 — Activează GitHub Pages
1. Mergi la „Settings" → „Pages"
2. Sub „Source": selectează „Deploy from a branch"
3. Branch: `main`, folder: `/ (root)`
4. Click „Save"

### Pas 5 — Accesează URL-ul
GitHub îți dă un link de forma:
```
https://NUMELE_TAU.github.io/traducator-claude/
```
Acesta este URL-ul aplicației tale.

---

## Metoda 2: Netlify Drop (cel mai rapid, fără cont)

1. Mergi la → https://app.netlify.com/drop
2. Trage ÎNTREGUL folder `translator-pwa` pe pagina respectivă
3. Netlify îți dă instant un URL public
4. Gata!

---

## Instalarea pe iPhone / iPad

1. **Deschide URL-ul** în **Safari** (obligatoriu Safari, nu Chrome/Firefox)
2. Apasă butonul **Share** (pătratul cu săgeată în sus ↑) din bara de jos
3. Scroll jos în lista de opțiuni → **„Add to Home Screen"**
4. Confirmă cu **„Add"**

Aplicația apare pe ecranul de start cu iconița sa, exact ca o aplicație nativă.
La deschidere, rulează fără bara de adrese (fullscreen-like).

---

## La prima utilizare

Aplicația cere **cheia API Anthropic**:
- Obții cheia de la: https://console.anthropic.com → API Keys → Create Key
- Arată astfel: `sk-ant-api03-...`
- Se salvează local pe telefon (localStorage), nu este transmisă nicăieri altundeva

---

## Funcționează offline?

Interfața funcționează offline (cached prin Service Worker).
Traducerile necesită conexiune la internet (apelul către Claude API).
