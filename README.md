# **Git & GitHub Cheat Sheet**

## **1. Lokale Git-Einführung**

### **1.1 Git Repository initialisieren**
Ein neues Git-Repository anlegen:
```bash
git init
```
🔹 Erstellt einen versteckten Ordner `.git`, der die gesamte Versionshistorie speichert.

### **1.2 Status der Dateien überprüfen**
Zeigt den aktuellen Status der Dateien im Arbeitsverzeichnis:
```bash
git status
```
🔹 Zeigt unversionierte, geänderte oder zum Commit vorgemerkte Dateien.

### **1.3 Dateien dem Staging-Bereich hinzufügen**
Eine einzelne Datei hinzufügen:
```bash
git add <dateiname>
```
Alle geänderten Dateien hinzufügen:
```bash
git add .
```
🔹 `git add` speichert Änderungen im Staging-Bereich, aber noch nicht im Repository.

### **1.4 Änderungen committen**
Änderungen dauerhaft im Repository speichern:
```bash
git commit -m "Beschreibung der Änderung"
```
🔹 Commits sollten eine prägnante, erklärende Nachricht enthalten.

### **1.5 Änderungen in der Historie ansehen**
Alle bisherigen Commits anzeigen:
```bash
git log
```
Kompakte Ansicht:
```bash
git log --oneline --graph
```
🔹 Zeigt eine kürzere Darstellung der Commit-Historie.

### **1.6 Unterschiede anzeigen**
Unterschiede zwischen Arbeitsverzeichnis und Staging-Bereich:
```bash
git diff
```
Unterschiede zwischen Staging-Bereich und letztem Commit:
```bash
git diff --staged
```

---

## **2. GitHub & Verbindung mit lokalem Repository**

### **2.1 Repository von GitHub klonen**
Ein bestehendes GitHub-Repository auf den lokalen Rechner kopieren:
```bash
git clone <repository-url>
```
🔹 Erstellt eine lokale Kopie des Repositories mit der gesamten Historie.

### **2.2 Remote-Repository hinzufügen**
Ein lokales Repository mit GitHub verknüpfen:
```bash
git remote add origin <repository-url>
```
🔹 `origin` ist der Standardname für das entfernte Repository.

### **2.3 Änderungen zu GitHub hochladen (Push)**
Dateien nach GitHub senden:
```bash
git push -u origin main
```
🔹 `-u` setzt die Verknüpfung, sodass künftige `git push` ohne zusätzliche Parameter funktioniert.

### **2.4 Änderungen aus GitHub abrufen**
Neueste Änderungen herunterladen, ohne sie zu mergen:
```bash
git fetch
```
Neueste Änderungen abrufen und mit dem aktuellen Branch mergen:
```bash
git pull
```
🔹 `git pull` kombiniert `git fetch` und `git merge`.

---

## **3. Branches & Pull Requests**

### **3.1 Arbeiten mit Branches**
Einen neuen Branch erstellen:
```bash
git branch feature-xyz
```
In einen anderen Branch wechseln:
```bash
git checkout feature-xyz
```
Neuen Branch erstellen und direkt wechseln:
```bash
git checkout -b feature-xyz
```
🔹 Branches ermöglichen parallele Entwicklungen, ohne den `main`-Branch zu beeinflussen.

### **3.2 Änderungen in den Haupt-Branch mergen**
Zurück zum Haupt-Branch wechseln:
```bash
git checkout main
```
Den Feature-Branch in `main` mergen:
```bash
git merge feature-xyz
```

### **3.3 Merge-Konflikte lösen**
Falls Änderungen in beiden Branches kollidieren, muss der Konflikt manuell behoben werden:
1. Git zeigt betroffene Dateien mit Konfliktstellen (`<<<<<<<`, `=======`, `>>>>>>>`).
2. Konflikte manuell editieren und bereinigen.
3. Datei erneut zum Staging-Bereich hinzufügen:
   ```bash
   git add <dateiname>
   ```
4. Merge abschließen:
   ```bash
   git commit -m "Merge-Konflikte gelöst"
   ```

### **3.4 Pull Requests (PRs) auf GitHub erstellen**
1. Änderungen in einem separaten Branch committen und pushen:
   ```bash
   git push origin feature-xyz
   ```
2. Auf GitHub eine Pull-Request (PR) erstellen.
3. Änderungen überprüfen und ggf. Diskussion führen.
4. PR in `main` mergen.

🔹 PRs sind besonders wichtig für Zusammenarbeit in Teams, da sie vor dem Merge überprüft werden können.

---

🚀 **Mit diesen Git- und GitHub-Befehlen bist du bestens für die Versionskontrolle gewappnet!**
