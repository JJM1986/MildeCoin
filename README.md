# MildeCoin (MLDE)

**MildeCoin** ist ein BRC-20 Token auf der Bitcoin Blockchain.

## Token Details

| Parameter | Wert |
|-----------|------|
| Name | MildeCoin |
| Ticker | MLDE |
| Standard | BRC-20 |
| Netzwerk | Bitcoin |
| Max. Supply | 21.000.000 |
| Mint Limit | 1.000 pro Transaktion |

## BRC-20 Deploy Inscription

```json
{
  "p": "brc-20",
  "op": "deploy",
  "tick": "MLDE",
  "max": "21000000",
  "lim": "1000"
}
```

## BRC-20 Mint Inscription

```json
{
  "p": "brc-20",
  "op": "mint",
  "tick": "MLDE",
  "amt": "1000"
}
```

## BRC-20 Transfer Inscription

```json
{
  "p": "brc-20",
  "op": "transfer",
  "tick": "MLDE",
  "amt": "100"
}
```

## Deployment Guide

1. Installiere [Unisat Wallet](https://unisat.io) oder [Xverse](https://www.xverse.app)
2. Lade BTC auf deine Wallet (mind. 0.01 BTC für Gebühren)
3. Gehe zu [unisat.io/inscribe](https://unisat.io/inscribe)
4. Wähle "Inscribe BRC-20" → "Deploy"
5. Füge den Deploy JSON-Code ein und bestätige die Transaktion

## Ressourcen

- [Unisat Wallet](https://unisat.io)
- [Xverse Wallet](https://www.xverse.app)
- [BRC-20 Explorer](https://unisat.io/brc20)
- [Ordinals Explorer](https://ordinals.com)

## Lizenz

MIT
