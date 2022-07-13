# GIT-Befehle
1. **git config --global user.name "Name"** - setze oder ändere den Benutzernamen, der in Git angezeigt werden soll.
2. **git config --global user.email "myemail@mail.com"** setze oder ändere die in git gespeicherte E-Mail-Adresse
3. **git init** - Initialisierung des Repositorys
4. **git status** – überprüft den Status des Repositorys
5. **git add filname.ext** oder **git add .** – fügt einzelne Dateien oder alle Dateien zum Staging-Bereich hinzu
6. **git commit -m "Message About Commit"** - erstelle ein Commit
7. **git log** – Zeigt den Commit-Verlauf mit Änderungen an
8. **git diff** – Änderungen vor dem Commit anzeigen
9. **git checkout _<BranchName oder die ersten Zeichen des Commit-Hashes>_** – Springe zum angegebenen Branch oder Commit
10. **git checkout -b new_branch_name** – erstelle einen neuen Branch und wechsle zu ihm
11. **git branch new_branch_name** – erstelle einen neuen Branch
13. **git branch** – Liste der Branches anzeigen
14. **git branch -d branch_to_delete** – Lösche einen Zweig, ohne etwas zu beschädigen
15. **git merge branch_name** – Zusammenführen des angegebenen Zweigs mit dem aktuellen
16. **git log --graph** – Verzweigungsprotokoll als Diagramm anzeigen

*Wenn Sie eine **.gitignore**-Datei im Repository erstellen und dort eine Liste von Dateien hinzufügen, z. B. Bilder oder große Dateien, wenn Sie die **.gitignore**-Datei zum Repository hinzufügen, verarbeitet Git diese nicht Dateien

**git log -n** Zeigt die letzten n Commits an

**git log --seit 2022-01-17 _bis 2022-01-22_** Commits von einem bestimmten Datum *bis zu einem bestimmten Datum anzeigen (optional)*

**git rm _FileName_** Datei aus Git-Indizes entfernen

**git rebase main** kopiert eine Reihe von Commits und verschiebt sie an einen anderen Ort

**git trennt HEAD ab** trennt HEAD vom Branch zum Commit

**git checkout main^** schalte eine Ebene höher

**git checkout main~3** schiebe 3 Commits zurück

**git branch -f main HEAD~3** zwingt die Eltern des Hauptzweigs 3 zurück von HEAD


***
# Pushen des lokalen Repositorys auf den GitHub-Server

**Git-Remote-Ursprung hinzufügen <_WebPatch.git_>**

**git branch -M main**

**git push -u origin main**

**git push** Push-Änderungen an GitHub (_REQUIRES AUTHORIZATION_)

**git pull** vom Server herunterladen. Versucht zusammenzuführen

**?git fetch** lokalen Branch mit Remote synchronisieren. Git pull ruft git fetch gefolgt von git merge auf
***
# Git-Pull-Request

- Einen **Fork** (Zweig) des Repositorys erstellen
- Erstellen Sie einen Git-Klon von **unserer** Version des Repositorys
- Erstellen Sie einen neuen Zweig und **er** nimmt unsere Änderungen vor
- Änderungen beheben (Commits vornehmen)
- Senden Sie Ihre Version an Ihren GitHub
- Klicken Sie auf der GitHub-Website auf die Schaltfläche **Pull Request**
***