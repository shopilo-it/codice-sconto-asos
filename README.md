# Codice sconto ASOS, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto ASOS** da [shopilo.it](https://shopilo.it/negozi/asos.com). Restituisce **coupon ASOS** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-asos](https://shopilo-it.github.io/codice-sconto-asos/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-asos
cd codice-sconto-asos
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "ASOS",
    "code": "SHOPILO20",
    "discount": "20%",
    "description": "20% di sconto su abbigliamento selezionato",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/asos.com"
  }
]
```

## Coupon ASOS disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 20% | 20% di sconto su abbigliamento selezionato | [shopilo.it](https://shopilo.it/negozi/asos.com) |

Codici attivi: **[shopilo.it/negozi/asos.com](https://shopilo.it/negozi/asos.com)**

## Domande frequenti

### Come utilizzo un codice sconto ASOS?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/asos.com), aggiungi i prodotti al carrello su ASOS e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon ASOS?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher ASOS piu recenti?
La pagina [shopilo.it/negozi/asos.com](https://shopilo.it/negozi/asos.com) viene aggiornata quotidianamente con i codici sconto ASOS, voucher ASOS e coupon promozionali ASOS piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su ASOS

ASOS e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/asos.com) trovi i migliori codici sconto ASOS, coupon ASOS verificati e voucher ASOS attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-asos
```

```javascript
const { fetchCoupons } = require('codice-sconto-asos');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
