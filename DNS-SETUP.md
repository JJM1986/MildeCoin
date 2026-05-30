# MildeCoin — Custom Domain Setup (GitHub Pages)

Diese Anleitung erklärt Schritt für Schritt, wie du `mildecoin.com` mit deiner GitHub Pages Seite verbindest.

---

## Schritt 1: Domain kaufen

Empfehlung: **Namecheap** (akzeptiert auch Bitcoin!)

- [mildecoin.com bei Namecheap prüfen](https://www.namecheap.com/domains/registration/results/?domain=mildecoin.com)
- [mildecoin.io bei Namecheap prüfen](https://www.namecheap.com/domains/registration/results/?domain=mildecoin.io)
- [mildecoin.xyz bei Namecheap prüfen](https://www.namecheap.com/domains/registration/results/?domain=mildecoin.xyz)

---

## Schritt 2: DNS-Einträge setzen

### Bei Namecheap

1. Login auf [namecheap.com](https://namecheap.com)
2. Klicke auf **Domain List** → **Manage** neben deiner Domain
3. Klicke auf den Tab **Advanced DNS**
4. Lösche alle bestehenden A- und CNAME-Einträge
5. Füge folgende Einträge hinzu:

| Typ | Host | Wert | TTL |
|-----|------|------|-----|
| A | @ | 185.199.108.153 | Automatic |
| A | @ | 185.199.109.153 | Automatic |
| A | @ | 185.199.110.153 | Automatic |
| A | @ | 185.199.111.153 | Automatic |
| CNAME | www | jjm1986.github.io | Automatic |

### Bei GoDaddy

1. Login auf [godaddy.com](https://godaddy.com)
2. Gehe zu **My Products** → **DNS** neben deiner Domain
3. Bearbeite den bestehenden A-Eintrag und füge alle 4 GitHub IPs hinzu
4. Füge den CNAME-Eintrag für `www` hinzu (Wert: `jjm1986.github.io`)

### Bei anderen Anbietern

Die Einträge sind bei allen Anbietern gleich — nur die Oberfläche unterscheidet sich. Suche nach "DNS Management" oder "DNS Zone Editor".

---

## Schritt 3: Custom Domain in GitHub eintragen

1. Gehe zu: [github.com/JJM1986/MildeCoin/settings/pages](https://github.com/JJM1986/MildeCoin/settings/pages)
2. Scrolle zu **Custom domain**
3. Trage ein: `mildecoin.com`
4. Klicke auf **Save**
5. GitHub prüft nun automatisch die DNS-Einträge (grüner Haken = alles korrekt)

---

## Schritt 4: HTTPS aktivieren

1. Warte bis der grüne Haken bei "Custom domain" erscheint (~10 Minuten bis 24 Stunden)
2. Hake **Enforce HTTPS** an
3. GitHub stellt automatisch ein kostenloses SSL-Zertifikat aus (Let's Encrypt)

---

## Schritt 5: Warten & prüfen

DNS-Änderungen brauchen **bis zu 48 Stunden** bis sie weltweit aktiv sind.

Du kannst den Status prüfen unter:
- [dnschecker.org](https://dnschecker.org/#A/mildecoin.com) — zeigt ob die A-Einträge weltweit aktiv sind
- [whatsmydns.net](https://www.whatsmydns.net/#A/mildecoin.com) — alternative DNS-Prüfung

---

## Fertig! 🎉

Nach erfolgreicher Einrichtung ist deine MildeCoin Landingpage erreichbar unter:

- **https://mildecoin.com**
- **https://www.mildecoin.com**

---

## Häufige Probleme

| Problem | Lösung |
|---------|--------|
| GitHub zeigt "DNS check unsuccessful" | Warte 30 Minuten, dann erneut prüfen |
| Seite lädt nicht nach 48h | DNS-Einträge nochmal kontrollieren |
| HTTPS nicht verfügbar | Zuerst ohne HTTPS testen, dann aktivieren |
| Weiterleitung funktioniert nicht | CNAME-Eintrag für `www` prüfen |

---

## Nützliche Links

- [GitHub Pages Dokumentation](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)
- [DNS Checker](https://dnschecker.org)
- [Namecheap DNS Anleitung](https://www.namecheap.com/support/knowledgebase/article.aspx/9645/2208/how-do-i-link-my-domain-to-github-pages/)

---

*MildeCoin (MLDE) — github.com/JJM1986/MildeCoin*
