@AGENTS.md

### Remote-Freigabe: Claude darf in diesem Projekt pushen — jedes Mal erst auf ein Ja

*(Betreiber-Entscheid 2026-11-09)*

Diese Regel geht der Stufe 2 der globalen Git-Regel vor. Dies ist der Fork `jaeggin/threadbear`
(`origin`), `upstream` ist Mikes Repo und wird nie beschrieben.

**Freigegeben, aber jedes Mal erst nach Rückfrage:** `git push origin main` (und andere Branches nach
`origin`). Vor jedem Push wird gesagt, **was** rausgeht (Branch, Anzahl Commits) und die Antwort
abgewartet. Ein Ja gilt für diesen einen Vorgang, nicht für den nächsten.

**Lokale Commits und `tb land` brauchen keine Zustimmung**, sie verlassen den Rechner nicht.
**Lesen bleibt frei** (`git fetch`, `gh pr view`, `gh run view`, `gh api` mit `GET`).

**Weiterhin nur auf Zuruf im Einzelfall (Stufe 3):** `gh pr merge`, Force-Push, Remote-Branches
löschen, `gh workflow run`, Releases, `gh auth`, jede schreibende `gh api`, und alles gegen `upstream`.

Nach einem Push die URL oder den Stand von `origin/main` melden.
