# **Hausaufgabe: Git & GitHub**

## **Ziel der Aufgabe**
Diese Hausaufgabe soll dir helfen, das Arbeiten mit Git und GitHub weiter zu vertiefen. Die Aufgaben umfassen lokale Git-Befehle, das Arbeiten mit Branches sowie den Umgang mit Remote-Repositories auf GitHub.

---

## **1. Einrichtung eines lokalen Git-Repositories**

1. Erstelle einen neuen Ordner mit dem Namen `git-hausaufgabe`.
2. Wechsle in diesen Ordner (`cd git-hausaufgabe`).
3. Initialisiere ein neues Git-Repository (`git init`).
4. Erstelle eine Datei `tagebuch.md` und schreibe ein paar Sätze hinein.
5. Speichere die Datei und überprüfe den Status mit `git status`.
6. Füge die Datei zum Staging-Bereich hinzu (`git add tagebuch.md`).
7. Erstelle einen Commit mit der Nachricht `Erster Eintrag im Tagebuch` (`git commit -m "Erster Eintrag im Tagebuch"`).
8. Prüfe mit `git log`, ob dein Commit korrekt gespeichert wurde.

---


## **2. Verbindung mit GitHub**

1. Erstelle ein neues Repository auf GitHub (ohne README, `.gitignore` oder Lizenzdateien).
2. Verbinde dein lokales Repository mit GitHub:
   ```bash
   git remote add origin <URL-deines-GitHub-Repos>
   ```
3. Lade deine Änderungen nach GitHub hoch:
   ```bash
   git push -u origin master
   ```
---


🚀 **Mit dieser Hausaufgabe übst du die wichtigsten Git- und GitHub-Konzepte! Viel Erfolg!**
