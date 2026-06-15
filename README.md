# Segnalazione Veicoli via QR

Sistema leggero per la **tracciabilità della flotta** di FS Busitalia: ogni veicolo espone un QR code; chi lo inquadra può segnalare in pochi secondi quale mezzo sta utilizzando, indicando il proprio codice identificativo, con data/ora e posizione rilevate automaticamente.

🔗 **Pagina live:** https://gvasta62.github.io/bus-qr-segnalazione/

## Come funziona

1. L'operatore inquadra con lo smartphone il QR applicato sul veicolo — si apre questa pagina web (nessuna app da installare).
2. Inserisce il proprio **codice matricola (CID)** a 7 cifre, obbligatorio.
3. La pagina rileva in automatico **data/ora reali** e **posizione GPS** (previo consenso).
4. L'operatore sceglie il canale — **WhatsApp** oppure **Email** — e invia il messaggio già precompilato.

Il numero del veicolo viaggia nell'indirizzo della pagina (`?n=<matricola>`): un'unica pagina serve quindi l'intera flotta, una etichetta QR per ciascun mezzo.

## Contenuto di questo repository

Questo repository contiene **solo la pagina web pubblica** (`index.html`), ospitata tramite GitHub Pages.

L'elaborazione delle segnalazioni (raccolta dai canali, incrocio con l'anagrafica, registrazione su foglio di calcolo, notifiche) avviene in un **componente privato** che gira localmente e **non è incluso** in questo repository: registro, anagrafica, recapiti e credenziali non sono pubblicati, a tutela dei dati personali.

## Tecnologie

- HTML + JavaScript statici
- GitHub Pages (HTTPS)
- Geolocation API del browser
- Collegamenti `wa.me` (WhatsApp) e `mailto` (Email)

## Privacy

La pagina pubblica contiene esclusivamente il modulo di segnalazione. Nessun dato personale degli operatori è presente in questo repository.

---

*Progetto interno FS Busitalia · 2026*
