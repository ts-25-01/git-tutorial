# **Git & GitHub Exercises**

## **1. Lokale Git-Einführung**

### **1.1 Git Repository initialisieren**
Ein neues Git-Repository anlegen:
```bash
git init
```
🔹 Erstellt einen versteckten Ordner `.git`, der die gesamte Versionshistorie speichert.

#### **📝 Aufgabe:**
1. Erstelle einen neuen Ordner mit dem Namen `mein-projekt`.
2. Wechsle in diesen Ordner mit `cd mein-projekt`.
3. Initialisiere ein neues Git-Repository mit `git init`.
4. Überprüfe, ob der `.git`-Ordner erstellt wurde.

---

### **1.2 Status der Dateien überprüfen**
Zeigt den aktuellen Status der Dateien im Arbeitsverzeichnis:
```bash
git status
```
🔹 Zeigt unversionierte, geänderte oder zum Commit vorgemerkte Dateien.

#### **📝 Aufgabe:**
1. Erstelle eine neue Datei `notizen.txt` im Ordner `mein-projekt`.
2. Führe den Befehl `git status` aus und beobachte die Ausgabe.
3. Was sagt Git über die Datei `notizen.txt`?

---

### **1.3 Dateien dem Staging-Bereich hinzufügen**
Eine einzelne Datei hinzufügen:
```bash
git add <dateiname>
```

#### **📝 Aufgabe:**
1. Füge die Datei `notizen.txt` mit `git add notizen.txt` zum Staging-Bereich hinzu.
2. Überprüfe mit `git status`, ob die Datei nun im Staging-Bereich ist.

**Zusatzaufgabe:**
- Erstelle eine zweite Datei `todo.txt` und füge sie mit `git add .` zum Staging-Bereich hinzu.
- Überprüfe mit `git status`, ob alle Dateien aufgenommen wurden.

---

### **1.4 Änderungen committen**
Änderungen dauerhaft im Repository speichern:
```bash
git commit -m "Beschreibung der Änderung"
```

#### **📝 Aufgabe:**
1. Führe einen Commit mit der Nachricht `Initial commit` aus.
2. Überprüfe mit `git log`, ob der Commit erfolgreich war.

**Zusatzaufgabe:**
- Füge eine dritte Datei `readme.md` hinzu, committe sie mit einer passenden Nachricht und überprüfe deine Git-Historie mit `git log --oneline`.

---

### **1.5 Änderungen in der Historie ansehen**
Alle bisherigen Commits anzeigen:
```bash
git log
```

#### **📝 Aufgabe:**
1. Erstelle mehrere Commits mit unterschiedlichen Änderungen.
2. Verwende `git log`, um die Änderungen nachzuvollziehen.

**Zusatzaufgabe:**
- Nutze `git log --oneline --graph`, um die Historie in kompakter Form anzuzeigen.

---

### **2. GitHub & Verbindung mit lokalem Repository**

### **2.1 Repository von GitHub klonen**
Ein bestehendes GitHub-Repository auf den lokalen Rechner kopieren:
```bash
git clone <repository-url>
```

#### **📝 Aufgabe:**
1. Klone ein öffentliches GitHub-Repository auf deinen Rechner.
2. Wechsle in das geklonte Repository und überprüfe die enthaltenen Dateien.

**Zusatzaufgabe:**
- Untersuche mit `git remote -v`, welche Verbindungen zu GitHub bestehen.

---

### **2.3 Änderungen zu GitHub hochladen (Push)**
Dateien nach GitHub senden:
```bash
git push -u origin master
```

#### **📝 Aufgabe:**
1. Erstelle ein neues Repository auf GitHub. (Achtung: gib 'repo.new' in die Browser-Leiste ein). Wähle einen Namen und einen Owner aus. Lasse ansonsten alles auf default.
2. Verbinde dein lokales Repository mit GitHub (`git remote add origin <URL>`). Den Befehl siehst du auch ganz unten auf der Seite, die sich nach dem Erstellen des Repos geöffnet hat.
3. Führe `git push -u origin master` aus, um deine Änderungen hochzuladen.

**Zusatzaufgabe:**
- Erstelle einen neuen Branch `feature/xyz`, pushe diesen zu GitHub und überprüfe ihn im Web-Interface.

---

### **3. Branches & Pull Requests**

### **3.1 Arbeiten mit Branches**
Einen neuen Branch erstellen:
```bash
git branch feature-xyz
```

#### **📝 Aufgabe:**
1. Erstelle einen neuen Branch `experiment`.
2. Wechsle in diesen Branch mit `git checkout experiment`.
3. Erstelle eine neue Datei und committe sie in diesem Branch.

**Zusatzaufgabe:**
- Wechsel zurück zum `main`-Branch und merge den `experiment`-Branch.

---

### **3.3 Merge-Konflikte lösen**
Falls Änderungen in beiden Branches kollidieren, muss der Konflikt manuell behoben werden:

#### **📝 Aufgabe:**
1. Erstelle zwei Branches, die dieselbe Datei bearbeiten.
2. Führe ein Merge durch und beobachte einen möglichen Konflikt.
3. Löse den Merge-Konflikt manuell und committe die bereinigte Datei.

---

🚀 **Mit diesen Aufgaben kannst du Git und GitHub Schritt für Schritt lernen und vertiefen!**
