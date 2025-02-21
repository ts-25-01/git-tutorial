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

## **3. Zusatz: Arbeiten mit Branches (lokal)**

1. Erstelle einen neuen Branch mit dem Namen `experimenteller-eintrag` (`git branch experimenteller-eintrag`).
2. Wechsle in diesen Branch (`git checkout experimenteller-eintrag`).
3. Füge eine neue Datei `ideen.md` hinzu und schreibe ein paar Notizen hinein.
4. Speichere die Datei und committe sie mit einer passenden Nachricht.
5. Wechsle zurück zum `master`-Branch (`git checkout master`).
6. Führe `git merge experimenteller-eintrag` aus, um die Änderungen aus dem Branch zu übernehmen.

**Zusatzaufgabe:** Falls es zu einem Merge-Konflikt kommt, löse ihn manuell und committe die bereinigte Version der Datei. D.h. die Dateien bearbeiten, adden, committen

---
## **4. Zusatz: Arbeiten mit Branches (Github)**

1. Erstelle einen neuen Branch `feature/update` lokal mit:
   ```bash
   git checkout -b feature/update
   ```
2. Bearbeite eine Datei oder füge eine neue hinzu, committe die Änderungen und pushe sie zurück nach GitHub.
  ```bash
  git add .
  git commit -m "änderungen beschreiben"
  git push -u origin feature/update
  ```
3. Wechsle zurück auf den Hauptbranch mit `git checkout master`

**Zusatzaufgabe**: Wie kann ich den feature-Branch in meinen Hauptbranch mergen/zusammenführen? Hier gibt es verschiedene Möglichkeiten. Recherchiere und teste etwas aus :)

---

🚀 **Mit dieser Hausaufgabe übst du die wichtigsten Git- und GitHub-Konzepte! Viel Erfolg!**
