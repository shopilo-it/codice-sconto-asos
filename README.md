# Cod reducere ASOS — fetch automat de pe shopilo.it

Modul Python pentru fetch automat de **coduri de reducere ASOS** de pe [shopilo.it](https://shopilo.it/magazin/asos.com). Returneaza **cupoane ASOS** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-it.github.io/codice-sconto-asos](https://shopilo-it.github.io/codice-sconto-asos/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-asos
cd codice-sconto-asos
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "ASOS",
    "code": "SHOPILO20",
    "discount": "20%",
    "description": "20% di sconto su abbigliamento selezionato",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/magazin/asos.com"
  }
]
```

## Cupoane ASOS disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 20% | 20% di sconto su abbigliamento selezionato | [shopilo.it](https://shopilo.it/magazin/asos.com) |

Codurile active: **[shopilo.it/magazin/asos.com](https://shopilo.it/magazin/asos.com)**

## Intrebari frecvente

### Cum folosesc un cod de reducere ASOS?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.it](https://shopilo.it/magazin/asos.com), adauga produsele in cos pe ASOS, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele ASOS?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri ASOS?
Pagina [shopilo.it/magazin/asos.com](https://shopilo.it/magazin/asos.com) este actualizata zilnic cu cele mai noi cod reducere ASOS, voucher ASOS si cupon promotional ASOS.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre ASOS

ASOS este unul dintre magazinele online populare. Gasesti pe [shopilo.it](https://shopilo.it/magazin/asos.com) cele mai bune cod reducere ASOS, cupoane ASOS verificate si voucher ASOS active, actualizate zilnic.

## Instalare npm

```bash
npm install codice-sconto-asos
```

```javascript
const { fetchCoupons } = require('codice-sconto-asos');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.it](https://shopilo.it)
