# Over The Wall — Landing Page

Landing page a pagina singola (link-in-bio / bento grid) per il podcast **Over The Wall**.
HTML statico + Tailwind CSS (CDN). Nessuna build necessaria.

## Struttura cartella

```
landing page/
├── index.html              ← la pagina (apri questo)
├── favicon.png             ← icona scheda browser
├── README.md
└── assets/
    ├── logo-light.png      ← logo trasparente (WALL nero) per sfondi chiari
    ├── logo-dark.png       ← logo trasparente (WALL bianco) per sfondi scuri
    ├── wall.jpg            ← texture muro mattonato
    └── source/             ← file originali ad alta risoluzione (non usati dal sito)
```

## Anteprima locale

Apri `index.html` nel browser, oppure servi la cartella:

```bash
python -m http.server 8080
# poi apri http://localhost:8080
```

## Pubblicazione online

Sito 100% statico: caricabile su qualsiasi hosting.

**Opzioni consigliate (gratis, con dominio personalizzato):**
- **Netlify** — trascina la cartella su app.netlify.com → assegna il dominio in *Domain settings*.
- **Vercel** — `vercel` da terminale, oppure import del repo.
- **Cloudflare Pages** / **GitHub Pages** — collega il repo.
- **Hosting classico (cPanel/FTP)** — carica tutto il contenuto della cartella nella `public_html`.

### Prima di pubblicare
1. Nel `<head>` di `index.html` sostituisci `https://tuodominio.com` con il dominio reale (tag `canonical`, `og:*`, `twitter:*`).
2. Collega il dominio dal pannello dell'hosting (DNS: record A/CNAME forniti dal provider).

## Link configurati
- YouTube, Spotify, TikTok, Instagram → profili ufficiali
- Racconta la tua storia → Google Form
- Sostieni il progetto → GoFundMe
- Contatti → info@overthewallpodcast.com (copia + mailto)

## Note
- Tailwind è caricato via CDN: serve connessione internet. Per un sito totalmente offline/ottimizzato, compilare Tailwind in un CSS statico.
