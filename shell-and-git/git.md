# Git & GitHub

- **Git**: Versionierung auf Computer, die alle Änderungen sichtbar macht  
  vs.  
  **GitHub**: hochladen von Repositories oder Commits
- erst lokal arbeiten und wann immer nötig, hochladen
- kein Repo in Repo eröffnen

## Git local

- `git init` &rarr; Repo initialisieren
- `rm -rf .git` &rarr; Repo wieder löschen
- `.gitignore`-Datei erstellen, z.B. mit `DS_Store`
- `git status` &rarr; Status anzeigen lassen
- `git add <Datei>` oder `git add .` -> Änderungen stagen
- `git commit -m "commit-message"` &rarr; Änderungen commiten
- `git log` &rarr; Git Historie angucken, ggf. mit `--oneline`
- `git restore <Datei>` oder `git restore .` &rarr; Zurückseten auf letzten Commit
- `git remote -v` &rarr; überprüfen, ob es schon eine remote-Verknüpfung gibt
- `git remote add origin <sshlink>` &rarr; lokal mit remote verknüpft
- `git push -u origin main` &rarr; hochladen beim ersten Mal
- `git push` &rarr; hochladen

## Branches

- `git switch -c <branch-name>` &rarr; neuen Branch erstellen
- `git switch main` &rarr; Wechsel in anderen Branch, hier in main
- `git switch .` &rarr; Wechsel in Branch, wo wir davor waren
- pushen wie gehabt. Beim ersten Mal mit `-u origin <branch>`, dann ohne

## auf GitHub

- in Repository: button "Compare and pull request"
- PR: Anfrage, ob Branch in main übernommen werden kann
- merge (verschmelzen mit main-Branch)

## zurück in Git

- in main-Branch wechseln
- git pull
- `git branch` &rarr; Was gibt's für branches?
- `git branch -d <branch-name>` &rarr; Branch löschen
- Repository möglichst sauber halten, also nach merge löschen  
  sowohl auf GitHub als auch lokal

## generell:

- immer zu Beginn der Arbeit `git pull` &rarr; Repository auf den neuesten Stand bringen
- merken: "Wir schreiben den Code für den heutigen Tag." :smile:
