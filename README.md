<p align="center"><img src="NaturaSi_Category_Suite_Logo.png" alt="NaturaSì × RELEX" width="460"></p>

# NaturaSì Relex Category Optimizer · V4.2.08 BETA

Strumento interno del Team B.U. Grocery di EcorNaturaSì per gli store planner di sede. Legge l'export RELEX di un negozio (.xlsx) e propone minimi, massimi e interventi di assortimento in cinque tab: Setup, Diagnostica, Razionalizzazione, Sviluppo e Rollout.

## Come si usa

1. Apri la pagina dell'app da computer, con un browser aggiornato. Da smartphone e tablet l'app mostra un avviso e non si apre.
2. Carica l'export RELEX del negozio.
3. Imposta nel Setup i giorni di consegna e i booster, poi lavora i tab.

L'export resta sul computer: l'app lo legge nel browser e non lo invia a nessun server. La connessione serve solo per le librerie che leggono e scrivono Excel e PDF (cdnjs) e per i caratteri (Google Fonts).

## File della repository

| File | A cosa serve |
|---|---|
| `index.html` | L'app, compattata per la pubblicazione |
| `NaturaSi_Category_Suite_Logo.svg` | Logo mostrato dall'app |
| `NaturaSi_Category_Suite_Logo.png`, `NaturaSi_Category_Suite_Logo.JPG` | Logo in formato immagine (il PNG è quello in cima a questa pagina) |
| `favicon.ico`, `favicon-16x16.png`, `favicon-32x32.png`, `apple-touch-icon.png` | Icone della scheda del browser e dei preferiti |
| `android-chrome-192x192.png`, `android-chrome-512x512.png`, `site.webmanifest` | Resto del pacchetto icone: l'app non li richiama, restano pronti per un collegamento sulla schermata Home |
| `LICENSE.txt` | Licenza d'uso |
| `.gitignore` | Evita di caricare per sbaglio export e dati dei negozi (.xlsx, .csv) |
| `.nojekyll` | Fa pubblicare a GitHub Pages i file così come sono |

## Il file index.html

È compattato: niente commenti né rientri, nomi interni accorciati, il codice su poche righe molto lunghe. Così non si legge a colpo d'occhio, ma non è cifrato né protetto. La versione leggibile, i manuali e i collaudi stanno nel pacchetto di sviluppo, fuori da questa repository.

## Licenza

Copyright (c) 2026 Massimo Maggipinto. Il know-how operativo e la logica di business incorporati sono proprietà di EcorNaturaSì S.p.A. Uso, copia e distribuzione sono regolati da [LICENSE.txt](LICENSE.txt).
