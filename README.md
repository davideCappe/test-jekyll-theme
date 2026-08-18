# Demo Jekyll Theme — Officina Digitale

Questo repository è una demo Jekyll che mostra diverse funzionalità: layout responsive, collections, pagine dinamiche, RSS, sitemap e base per ricerca client-side.

Se preferisci non installare gem localmente, puoi fare il deploy direttamente su GitHub Pages: GitHub costruirà il sito usando le impostazioni in `_config.yml`.

Per pubblicare su GitHub Pages (repository `davidecappe/test-jekyll-theme`) basta pushare sul ramo `gh-pages` o abilitare Pages dal ramo `main`/`master` e cartella `/(root)` o `/docs` a seconda della tua configurazione.

Se vuoi testare localmente, questi comandi sono utili (opzionale):

```powershell
gem install bundler
bundle install
bundle exec jekyll serve --livereload
```

Visita `http://127.0.0.1:4000` dopo l'avvio.

Note:

- `baseurl` in `_config.yml` è impostato su `/test-jekyll-theme` per funzionare con l'URL GitHub Pages `https://davidecappe.github.io/test-jekyll-theme/`.
- I plugin sono elencati in `_config.yml` e nel `Gemfile`, ma GitHub Pages li esegue da remoto: non è necessario installarli localmente per il deploy su Pages.
- Per aggiungere ricerca client-side si può integrare `lunr.js` e generare un index JSON.
