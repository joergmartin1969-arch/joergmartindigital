# Security-Checkliste (monatlich)

Datum: ____-__-__
Pruefer: ____________________

## 1) GitHub Security
- [ ] Security-Tab geprueft
- [ ] Keine offenen Dependabot-Alerts (oder Tickets erstellt)
- [ ] Secret Scanning und Push Protection weiterhin aktiv

## 2) GitHub Actions
- [ ] Unbekannte Actions geprueft (keine neuen Drittanbieter ohne Pruefung)
- [ ] Workflow permissions stehen auf "Read repository contents"
- [ ] "Allow GitHub Actions to create and approve pull requests" bleibt aus

## 3) Zugriff und Rechte
- [ ] Collaborators/Teams geprueft (nur noetige Personen)
- [ ] Alte Tokens/Apps/Deploy-Keys entfernt
- [ ] Branch Protection fuer main weiterhin aktiv

## 4) Lokaler Secret-Scan
PowerShell-Befehl:

```powershell
git grep -nEi "api[_-]?key|secret|token|password|passwd|private[_-]?key|BEGIN (RSA|OPENSSH|EC) PRIVATE KEY"
```

- [ ] Scan ausgefuehrt
- [ ] Treffer geprueft
- [ ] Falls Treffer: Secrets entfernt und Schluessel rotiert

## 5) Ergebnis
Status: [ ] OK  [ ] Nacharbeit noetig
Notizen:

- 
- 
- 
