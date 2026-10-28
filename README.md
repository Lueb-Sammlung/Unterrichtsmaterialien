# Mathematik – Unterrichtsmaterialien

Die Startseite baut sich **automatisch** aus den Ordnern. Du lädst nur Dateien hoch, und nach ein bis zwei Minuten stehen sie auf der Seite.

## So ist alles aufgebaut

```
Mathematik 5/            ← jeder Ordner wird ein Kasten auf der Seite
   links.txt             ← Internet-Links für diese Gruppe
   Wochenplan.pdf        ← Dateien direkt im Ordner
   Natürliche Zahlen/    ← Unterordner = Thema (Überschrift im Kasten)
      Escaperoom.html
Mathematik 6/
Mathematik Kurs/
seite_erstellen.py       ← baut die Seite (nicht ändern)
.github/workflows/       ← startet den Bau automatisch (nicht ändern)
```

- **Der Dateiname wird zum Titel auf der Seite.** `Brüche kürzen – Lösungen.pdf` erscheint als „Brüche kürzen – Lösungen“. Umlaute und Leerzeichen sind erlaubt.
- **Erlaubte Dateien:** HTML (Lernumgebungen), PDF, Word, PowerPoint, Excel, Bilder, GeoGebra (.ggb).
- **Reihenfolge festlegen:** Setz eine Zahl vor den Namen, z. B. `1 Natürliche Zahlen` und `2 Geometrie`. Die Zahl wird auf der Seite nicht angezeigt.
- **Links:** In `links.txt` steht ein Link pro Zeile: `Titel | https://adresse.de`

---

## Einmalig: Seite einrichten (ca. 10 Minuten)

**1. Repository anlegen**
Bei github.com anmelden → oben rechts **+** → **New repository**.
Als Name z. B. `mathe` eintragen, **Public** auswählen → **Create repository**.

**2. Ordner hochladen**
Auf der neuen Seite den Link **uploading an existing file** anklicken.
ZIP-Datei entpacken. Diese Ordner und Dateien ins Fenster ziehen:
`Mathematik 5`, `Mathematik 6`, `Mathematik Kurs`, `seite_erstellen.py`, `README.md`
→ unten **Commit changes**.

**3. GitHub Pages einschalten**
**Settings** → links **Pages** → unter *Source* **GitHub Actions** auswählen.
(Wichtig: nicht „Deploy from a branch“.)

**4. Automatik einrichten**
Zurück zur Startseite des Repositorys (oben auf `Code` klicken) → **Add file** → **Create new file**.
Als Dateinamen genau eintippen: `.github/workflows/seite.yml`
(Nach jedem `/` legt GitHub automatisch einen Ordner an.)
Die Datei `workflow-vorlage.txt` aus der ZIP öffnen, den ganzen Inhalt kopieren und ins große Feld einfügen → **Commit changes**.

**5. Fertig**
Unter **Actions** siehst du, wie die Seite gebaut wird. Ein grüner Haken bedeutet: fertig.
Deine Seite: `https://DEIN-BENUTZERNAME.github.io/mathe/`

---

## Neues Material hochladen

1. Im Repository den Ordner öffnen, z. B. `Mathematik 6`.
2. **Add file** → **Upload files** → Datei hineinziehen → **Commit changes**.
3. Ein bis zwei Minuten warten, dann die Seite neu laden.

**Neues Thema:** Leg auf deinem Computer einen Ordner an, z. B. `Bruchrechnung`, mit den Dateien darin. Zieh diesen Ordner in Schritt 2 ins Fenster.

**Link hinzufügen:** `links.txt` im passenden Ordner öffnen → Stift-Symbol → neue Zeile `Titel | https://…` → **Commit changes**.

**Datei löschen:** Datei anklicken → oben rechts **…** → **Delete file** → **Commit changes**.

---

## Gut zu wissen

- **Alles ist öffentlich.** Lade keine Schülerdaten oder Noten hoch, und nur Material, an dem du die Rechte hast (keine Scans aus Schulbüchern).
- **Seite nicht aktualisiert?** Unter **Actions** nachsehen. Ein rotes ✗ bedeutet einen Fehler, meistens fehlt dann Schritt 3.
- **Direkt zu einer Gruppe springen:** Die Knöpfe oben auf der Seite springen zum jeweiligen Kasten.
