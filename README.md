# Codice sconto Libraccio, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Libraccio** da [shopilo.it](https://shopilo.it/negozi/libraccio.it). Restituisce **coupon Libraccio** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-libraccio](https://shopilo-it.github.io/codice-sconto-libraccio/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-libraccio
cd codice-sconto-libraccio
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Libraccio",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su libri nuovi e usati",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/libraccio.it"
  }
]
```

## Coupon Libraccio disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su libri nuovi e usati | [shopilo.it](https://shopilo.it/negozi/libraccio.it) |

Codici attivi: **[shopilo.it/negozi/libraccio.it](https://shopilo.it/negozi/libraccio.it)**

## Domande frequenti

### Come utilizzo un codice sconto Libraccio?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/libraccio.it), aggiungi i prodotti al carrello su Libraccio e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Libraccio?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Libraccio piu recenti?
La pagina [shopilo.it/negozi/libraccio.it](https://shopilo.it/negozi/libraccio.it) viene aggiornata quotidianamente con i codici sconto Libraccio, voucher Libraccio e coupon promozionali Libraccio piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Libraccio

Libraccio e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/libraccio.it) trovi i migliori codici sconto Libraccio, coupon Libraccio verificati e voucher Libraccio attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-libraccio
```

```javascript
const { fetchCoupons } = require('codice-sconto-libraccio');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
