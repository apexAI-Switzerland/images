# 🔧 Verwendung des Repositories als Asset-Bibliothek

Dieses Repository wird als **öffentliche Mediathek** verwendet, um Bilder/Assets über **stabile Direkt-URLs** in externen Projekten (z. B. Framer, HTML-Mails, etc.) einzubinden.

## ✅ Vorgehen

### 1. Bild hochladen

1. Repository öffnen  
2. **→ Add file → Upload files**  
3. Bilddatei(en) hochladen  
4. **Commit changes** klicken

🔎 Die Datei liegt anschliessend unter:

https://github.com/<OWNER>/<REPO>/blob/main/<DATEINAME>

### 2. Raw-URL erstellen (öffentliche Direkt-URL)

Die obige Datei-URL wird wie folgt **umgewandelt**:

| Teil | Ersetzen durch |
|------|----------------|
| `github.com` | `raw.githubusercontent.com` |
| `/blob/` | `/` (einfach entfernen) |

**Beispiel:**

| GitHub-URL | Raw-URL |
|------------|--------|
| https://github.com/apexAI-Switzerland/images/blob/main/Haushaltsfee_ok.png | https://raw.githubusercontent.com/apexAI-Switzerland/images/main/Haushaltsfee_ok.png |

👉 Die Raw-URL lässt sich direkt in Framer oder HTML-Code verwenden.

---

### 🔁 Bild ersetzen (ohne neuen Link)

Damit die URL gleich bleibt:

- **Dateinamen unverändert lassen**
- Bild hochladen → beim Commit „**Commit directly to main**“ auswählen → das bestehende Bild wird überschrieben

📌 Dadurch wird das Bild aktualisiert, aber die URL ändert sich **nicht**.

---

### ❗ Wichtig

| Fall | Ergebnis |
|------|---------|
| Datei umbenannt | ❌ URL wird ungültig |
| Datei gelöscht | ❌ URL wird ungültig |
| Branch geändert | ❌ Raw-URL muss aktualisiert werden |

**→ immer auf `main` bleiben & Dateinamen konsequent beibehalten**

---

✅ Fertig – das Repository kann nun wie ein CDN verwendet werden.
