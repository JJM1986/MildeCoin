# MildeCoin (MLDE) — BRC-20 Deployment Guide

## Voraussetzungen

- Computer oder Laptop (kein Handy empfohlen)
- Chrome oder Firefox Browser
- Mindestens **0,02 BTC** für Inscription-Gebühren

---

## Schritt 1: Unisat Wallet installieren

1. Gehe zu [chromewebstore.google.com](https://chromewebstore.google.com)
2. Suche nach **"UniSat Wallet"**
3. Klicke auf "Zu Chrome hinzufügen"
4. Erstelle eine neue Wallet:
   - Klicke auf "Create new wallet"
   - Schreibe deine **Seed Phrase (12 Wörter)** auf Papier auf — NIEMALS digital speichern!
   - Bestätige die Seed Phrase
   - Setze ein sicheres Passwort

> ⚠️ **Wichtig:** Wer deine Seed Phrase hat, hat dein Geld. Bewahre sie sicher auf!

---

## Schritt 2: BTC einzahlen

1. Öffne UniSat Wallet (Klick auf das Extension-Icon)
2. Kopiere deine Bitcoin-Adresse (beginnt mit `bc1p...`)
3. Sende mindestens **0,02 BTC** von einer Exchange (z.B. Binance, Coinbase, Kraken) an diese Adresse
4. Warte auf **1 Bestätigung** (~10 Minuten)

---

## Schritt 3: Ticker-Verfügbarkeit prüfen

1. Gehe zu [unisat.io/brc20](https://unisat.io/brc20)
2. Suche nach **"MLDE"**
3. Wenn der Ticker frei ist → weiter zu Schritt 4
4. Falls belegt → alternativen Ticker wählen (z.B. `MILD`, `MLDC`, `MLDN`)

---

## Schritt 4: Token deployen

1. Gehe zu [unisat.io/inscribe](https://unisat.io/inscribe)
2. Verbinde deine UniSat Wallet (Klick auf "Connect Wallet")
3. Wähle **"BRC-20"** → **"Deploy"**
4. Füge folgenden JSON-Code ein:

```json
{
  "p": "brc-20",
  "op": "deploy",
  "tick": "MLDE",
  "max": "21000000",
  "lim": "1000"
}
```

5. Wähle eine **Gebührenstufe** (empfohlen: "Avg" oder "Fast")
6. Klicke auf **"Next"** → überprüfe alle Details
7. Klicke auf **"Pay & Submit"**
8. Bestätige die Transaktion in der UniSat Wallet

> ⏳ Warte auf die Bestätigung (~10–30 Minuten je nach Netzwerk-Auslastung)

---

## Schritt 5: Token minen (Mint)

Nach erfolgreichem Deploy kannst du Tokens minten:

1. Gehe wieder zu [unisat.io/inscribe](https://unisat.io/inscribe)
2. Wähle **"BRC-20"** → **"Mint"**
3. Gib den Ticker **MLDE** ein
4. Gib die Menge ein (max. **1000** pro Transaktion)
5. Klicke auf **"Next"** → **"Pay & Submit"**

Du kannst diesen Schritt beliebig oft wiederholen, bis die maximale Supply von **21.000.000 MLDE** erreicht ist.

---

## Schritt 6: Token übertragen

1. Gehe zu [unisat.io/inscribe](https://unisat.io/inscribe)
2. Wähle **"BRC-20"** → **"Transfer"**
3. Gib Ticker **MLDE**, Menge und die Empfänger-Bitcoin-Adresse ein
4. Bestätige die Transaktion

---

## Gebühren-Übersicht (ungefähre Werte)

| Aktion | Geschätzte Gebühr |
|--------|-------------------|
| Deploy | ~0,005–0,01 BTC |
| Mint (pro Transaktion) | ~0,001–0,003 BTC |
| Transfer | ~0,001–0,003 BTC |

> Gebühren variieren je nach Bitcoin-Netzwerk-Auslastung (Mempool).

---

## Nützliche Links

- [UniSat Wallet](https://unisat.io)
- [UniSat Inscribe](https://unisat.io/inscribe)
- [BRC-20 Explorer](https://unisat.io/brc20)
- [Ordinals Explorer](https://ordinals.com)
- [Mempool (Gebühren prüfen)](https://mempool.space)

---

## Häufige Fehler

| Problem | Lösung |
|---------|--------|
| Ticker bereits vergeben | Anderen Ticker wählen |
| Transaktion fehlgeschlagen | Höhere Gebühr wählen |
| Zu wenig BTC | Mehr BTC einzahlen |
| Wallet nicht verbunden | Browser neu starten, Wallet-Extension prüfen |

---

*Erstellt für das MildeCoin (MLDE) Projekt — github.com/JJM1986/MildeCoin*
