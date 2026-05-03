## Git Basics

Ich bin gerade im Branch b03. Git zeigt mir, dass ich zwei Dateien geändert habe, nämlich CONTRIBUTING.md und homework/b03.md, aber ich habe die Änderungen noch nicht mit git add hinzugefügt. Das heißt, Git sieht die Änderungen, aber sie sind noch nicht bereit für einen Commit.

Dann gibt es noch die Datei foo.java. Die steht bei „Untracked files“, das bedeutet, die Datei ist neu und Git verfolgt sie noch nicht, weil ich sie noch nicht hinzugefügt habe.

Unten steht, dass noch nichts zum Commit hinzugefügt wurde. Das heißt, ich kann gerade nichts committen, weil ich zuerst git add benutzen muss. Mit git add füge ich die Dateien zur Staging Area hinzu, also Git merkt sich dann, was ich beim nächsten Commit speichern will.

Es gibt auch den Hinweis mit discard bzw. git restore. Damit kann ich Änderungen wieder rückgängig machen. Das heißt, wenn ich eine Datei geändert habe und die Änderungen doch nicht will, kann ich sie damit verwerfen und auf den letzten Stand zurücksetzen.

Wenn ich nur foo.java committen will, mache ich einfach git add foo.java und danach git commit.

---

## Git Quest

Bei tag 01 ist Markus in den Dungeon gegangen und trifft auf die ersten Monster.

Der Held hat zum ersten Mal 4 experience Punkte bei tag 01.3.

Der Held hat zum ersten Mal 10 hunger Punkte bei tag 02.

Der Held hat insgesamt 2 Heiltränke bekommen, bei tag 03.14 und tag 04.4.

Im Shop hat er einen Heiltrank und ein Brot gekauft. Jedes hat 5 Gold gekostet.

Zwischen tag 03 und tag 04 hat er sich erholt, seine health ist wieder auf 10 gegangen und hunger auf 0. Außerdem hat er sein Gold ausgegeben.

Ja, der Held hat etwas gegessen. Er hat ein Brot gegessen bei tag 03.17.
