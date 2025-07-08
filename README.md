# 🛠️ Windows Keylogger mit automatischem Mailversand (Python)

Dieses Projekt zeigt, wie man einen einfachen Keylogger für Windows mit Python erstellt, der automatisch alle Tasteneingaben an eine E-Mail-Adresse sendet. **Das Projekt dient ausschließlich zu Bildungszwecken!**

## ⚠️ Hinweis  
Die Nutzung eines Keyloggers ohne ausdrückliche Zustimmung der betroffenen Person ist illegal. Bitte verwende dieses Projekt ausschließlich für Test- und Lernzwecke auf deinem eigenen System.

---

## 🔧 1. Vorbereitung (Installation der Voraussetzungen)

Bevor du mit dem eigentlichen Code startest, musst du folgende Tools und Einstellungen vorbereiten:

- **Python 3.11.2** installieren: [Python-Downloadseite](https://www.python.org/downloads/)
- **Sublime Text Editor** installieren: [Sublime Text](https://www.sublimetext.com/)
- Einen Ordner namens `Keylogger` anlegen
- Ein Zahnrad-Icon (`Gear`) von [icon-icons.com](https://icon-icons.com) herunterladen und im `Keylogger`-Ordner als `icon.ico` speichern
- Eine Datei namens `keylogger.py` in diesem Ordner erstellen
- **Windows Defender deaktivieren**, damit bei der Erstellung des Keyloggers keine Warnungen auftreten

---

## 📩 2. Gmail für den Log-Versand einrichten

Damit der Keylogger die gesammelten Tasteneingaben per Mail verschicken kann, musst du dein Gmail-Konto wie folgt vorbereiten:

1. Gehe in deinen Google-Account unter **Sicherheit**
2. Aktiviere die **Zwei-Faktor-Authentifizierung**
3. Suche nach dem Begriff **„App-Passwort“**
4. Wähle als Projektname z. B. **KeyLogger**
5. Kopiere das generierte **App-Passwort**, dieses wird später im Code verwendet

---

## 💻 3. Keylogger Code & Kompilierung

Jetzt kommt der eigentliche Code und die Erstellung der ausführbaren Datei:

1. Lade die `keylogger.py` aus diesem Repository herunter oder kopiere den Code in deine eigene `keylogger.py` im `Keylogger`-Ordner
2. Trage im Script deine Daten ein:
   - `from_email` = Deine Gmail-Adresse  
   - `to_email` = Empfänger-Adresse (kann auch deine eigene sein)  
   - `password` = Das zuvor generierte App-Passwort
3. Öffne PowerShell im Projektordner und führe folgenden Befehl aus, um das Script zu einer `.exe`-Datei zu kompilieren:
   ```bash
   pyinstaller -w -F keylogger.py --icon=icon.ico


## ♻️ 4. Automatischer Start beim Systemstart (Persistenz)
Dieser Teil wird noch entwickelt.
Ziel ist es, den Keylogger beim Systemstart automatisch ausführen zu lassen – z. B. durch einen Eintrag in die Windows-Registry oder im Autostart-Ordner.

## 📷 Ergebnis
(Hier kannst du 2–3 Screenshots einfügen, um das Endergebnis zu zeigen – z. B. die generierte .exe, den gesendeten E-Mail-Log oder die Funktionsweise im Hintergrund.)



<img width="1440" alt="Bildschirmfoto 2025-07-08 um 15 43 31" src="https://github.com/user-attachments/assets/739cb39d-e83f-497b-baa5-4278a6ef0406" />
Keylogger auf dem Rechner des Opfers abgelegt


E-Mail die die aufgenommenen Keystrokes an uns sendet.

