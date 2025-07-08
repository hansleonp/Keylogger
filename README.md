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
Keylogger persistent machen (Autostart einrichten)

- Die bereits auf dem Zielgerät platzierte .exe-Datei (Keylogger) vorbereiten
- Windows-Taste + R drücken, um den Ausführen-Dialog zu öffnen
- Folgenden Befehl eingeben und mit Enter bestätigen:

shell:startup

- Im geöffneten Autostart-Ordner eine Verknüpfung zur Keylogger-Datei einfügen
- Ergebnis: Bei jedem Systemstart wird der Keylogger automatisch ausgeführt

## 📷 Ergebnis


<img width="1440" alt="Bildschirmfoto 2025-07-08 um 15 43 31" src="https://github.com/user-attachments/assets/739cb39d-e83f-497b-baa5-4278a6ef0406" />
Keylogger auf dem Rechner des Opfers abgelegt durch eine Social Engineering Attacke.


<img width="1437" alt="Bildschirmfoto 2025-07-08 um 16 07 06" src="https://github.com/user-attachments/assets/e5149fae-93e2-4872-b8a3-66ca3fa325c5" />
Das Opfer surft ahnungslos im Internet und führt beispielweise eine Überweisung durch.

<img width="1384" alt="Bildschirmfoto 2025-07-08 um 16 02 07" src="https://github.com/user-attachments/assets/abeb0402-3de4-457b-9865-2274d56d1348" />
E-Mail die die aufgenommenen Keystrokes an uns sendet.

