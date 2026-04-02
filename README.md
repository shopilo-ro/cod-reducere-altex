# Cod reducere Altex — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere Altex** de pe [shopilo.ro](https://shopilo.ro/magazin/altex.ro). Returneaza **cupoane Altex** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-altex](https://shopilo-ro.github.io/cod-reducere-altex/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-altex
cd cod-reducere-altex
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Altex",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% reducere la electronice selectate",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/altex.ro"
  }
]
```

## Cupoane Altex disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 10% | 10% reducere la electronice selectate | [shopilo.ro](https://shopilo.ro/magazin/altex.ro) |

Codurile active: **[shopilo.ro/magazin/altex.ro](https://shopilo.ro/magazin/altex.ro)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Altex?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/altex.ro), adauga produsele in cos pe Altex, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Altex?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Altex?
Pagina [shopilo.ro/magazin/altex.ro](https://shopilo.ro/magazin/altex.ro) este actualizata zilnic cu cele mai noi cod reducere Altex, voucher Altex si cupon promotional Altex.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Altex

Altex este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/altex.ro) cele mai bune cod reducere Altex, cupoane Altex verificate si voucher Altex active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-altex
```

```javascript
const { fetchCoupons } = require('cod-reducere-altex');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
