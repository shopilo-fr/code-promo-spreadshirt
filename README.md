# Code promo Spreadshirt, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo Spreadshirt** depuis [shopilo.fr](https://shopilo.fr/reductions/spreadshirt.fr). Renvoie les **coupons Spreadshirt** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-spreadshirt](https://shopilo-fr.github.io/code-promo-spreadshirt/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-spreadshirt
cd code-promo-spreadshirt
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "Spreadshirt",
    "code": "SHOPILO20",
    "discount": "20%",
    "description": "20% de reduction sur les t-shirts personnalises",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/spreadshirt.fr"
  }
]
```

## Coupons Spreadshirt disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 20% | 20% de reduction sur les t-shirts personnalises | [shopilo.fr](https://shopilo.fr/reductions/spreadshirt.fr) |

Codes actifs : **[shopilo.fr/reductions/spreadshirt.fr](https://shopilo.fr/reductions/spreadshirt.fr)**

## Questions frequentes

### Comment utiliser un code promo Spreadshirt ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/spreadshirt.fr), ajoutez les produits a votre panier sur Spreadshirt et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons Spreadshirt ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction Spreadshirt les plus recents ?
La page [shopilo.fr/reductions/spreadshirt.fr](https://shopilo.fr/reductions/spreadshirt.fr) est mise a jour quotidiennement avec les codes promo Spreadshirt, bons de reduction Spreadshirt et coupons promotionnels Spreadshirt les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de Spreadshirt

Spreadshirt est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/spreadshirt.fr), retrouvez les meilleurs codes promo Spreadshirt, coupons Spreadshirt verifies et bons de reduction Spreadshirt actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-spreadshirt
```

```javascript
const { fetchCoupons } = require('code-promo-spreadshirt');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
