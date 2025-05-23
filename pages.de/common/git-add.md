# git add

> Füge Dateien zum Index/Stage hinzu.
> Weitere Informationen: <https://git-scm.com/docs/git-add>.

- Füge eine bestimmte Datei zum Index hinzu:

`git add {{pfad/zu/datei}}`

- Füge alle Dateien zum Index hinzu (nachverfolgte und nicht nachverfolgte):

`git add {{[-A|--all]}}`

- Füge nur nachverfolgte Dateien zum Index hinzu (Updaten des Index):

`git add {{[-u|--update]}}`

- Füge auch Dateien, welche ignoriert werden (`.gitignore`) hinzu:

`git add {{[-f|--force]}}`

- Füge Teile von Dateien zum Index interaktiv hinzu:

`git add {{[-p|--patch]}}`

- Füge Teile einer bestimmten Datei interaktiv hinzu:

`git add {{[-p|--patch]}} {{pfad/zu/datei}}`

- Füge Dateien zum Index interaktiv hinzu:

`git add {{[-i|--interactive]}}`
