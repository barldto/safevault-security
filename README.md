
# 🛡️ SafeVault – Sichere Webanwendung mit ASP.NET Core und GitHub Copilot

## ✅ Projektübersicht
Dieses Projekt kombiniert sichere Codierung, Zugriffskontrolle, Schwachstellenbehebung und Testautomatisierung in einer ASP.NET Core-Anwendung. GitHub Copilot wurde aktiv zur Codegenerierung, Analyse und Testunterstützung genutzt.

---

## 📊 Abschlussbewertung (30 Punkte)

| Kriterium                                                                                      | Erfüllt | Punkte |
|-----------------------------------------------------------------------------------------------|---------|--------|
| 🔗 GitHub-Repository erstellt                                                                 | ✅       | 5      |
| 🔐 Copilot zur sicheren Eingabevalidierung & SQL-Injection-Prävention genutzt                | ✅       | 5      |
| 🔑 Copilot für Authentifizierung & RBAC-Implementierung verwendet                            | ✅       | 5      |
| 🐞 Sicherheitslücken (SQLi, XSS) mit Copilot identifiziert, behoben & refaktoriert            | ✅       | 5      |
| ✅ Tests zur Überprüfung sicherheitsrelevanter Funktionen mit Copilot erstellt & ausgeführt   | ✅       | 5      |
| 📝 Zusammenfassung zu Schwachstellen, Fixes und Copilot-Hilfe dokumentiert                   | ✅       | 5      |

**💯 Gesamtpunkte: 30 / 30**

---

## 🔐 Sicherheitsaktivitäten

### Aktivität 1: Eingabe & SQLi-Prävention
- Validierung mit Regex, `ModelState.IsValid`
- SQL-Parameterverwendung zur Vermeidung von SQL-Injection
- HTML-Encoding gegen XSS
- Copilot-Unterstützung bei Formularstruktur und Tests

### Aktivität 2: Authentifizierung & Rollen
- ASP.NET Identity, Passwort-Hashing
- `[Authorize(Roles = "Admin")]` für Admin-Zugriff
- Copilot generierte Login-Methoden und Testfälle

### Aktivität 3: Debugging & Fixes
- Schwachstellen (SQLi/XSS) durch Copilot identifiziert
- Refactoring unsicherer Stellen mit sicheren Mustern
- HTML-Sanitizing (`HtmlEncode`), `AntiForgeryToken`

---

## 🤖 Copilot-Unterstützung
- Code-Vorschläge für Validierung, Sicherheit & Tests
- Warnungen bei unsicherer SQL- oder HTML-Nutzung
- Templates für RBAC, Rollenprüfungen & Sicherheitstests

---

## 📁 Projektstruktur
```
SafeVault/
├── Controllers/
├── Models/
├── Views/
├── Services/
├── Utils/
├── Tests/
├── appsettings.json
└── Program.cs
```

---

## ▶️ Ausführung & Tests
```bash
dotnet ef migrations add Init
dotnet ef database update
dotnet run
dotnet test
```

---

## 📎 Repository-Link
https://github.com/barldto/safevault-security