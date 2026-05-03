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


---

## Commit Meldung

Beim ersten Commit „Layer system 5“ versteht man nur ungefähr, worum es geht. Die Nachricht ist nicht sehr genau und es wirkt so, als wären mehrere Sachen in einem Commit geändert worden, zum Beispiel Layer-System, Rebase, Spotless und AbstractController. Das finde ich etwas unübersichtlich. Besser wäre eine genauere Nachricht wie „Add layer system to controller“ oder mehrere kleine Commits.

Beim zweiten Commit „[GAME] better Items and Crafting settings“ finde ich die Nachricht besser, weil man direkt sieht, dass es um Items und Crafting geht. Trotzdem ist auch dieser Commit etwas groß, weil mehrere Sachen gleichzeitig geändert wurden. Ich würde es besser finden, wenn Crafting-Rezepte und Item-Änderungen in getrennten Commits wären.


---
## Installation und Gradle

Ich habe JDK 25 installiert und mit java -version geprüft. Wichtig ist, dass in der Ausgabe Version 25 und LTS steht.

Als IDE benutze ich IntelliJ IDEA. Ich habe darauf geachtet, dass das Projekt mit Gradle gebaut und gestartet wird.

Ein neues Gradle-Projekt erstellt man mit gradle init. Dabei wählt man Java Application, Groovy als Build-Script und JUnit als Test-API aus.

Alle verfügbaren Gradle-Tasks kann man mit ./gradlew tasks anzeigen lassen. Unter Windows kann man auch gradlew.bat tasks benutzen.

Die Java-Dateien liegen in src/main/java und die Testdateien in src/test/java. Das Buildskript heißt build.gradle. Dort stehen die Plugins, Abhängigkeiten und Einstellungen für das Projekt.

Das Plugin application sorgt dafür, dass man das Java-Programm mit Gradle starten kann. Dadurch gibt es zum Beispiel den Task run. Weitere wichtige Tasks sind build, test und clean.

In IntelliJ kann man die Gradle-Tasks rechts im Gradle-Fenster starten.

Für das Semester habe ich ein Java-Projekt mit Gradle-Support angelegt. Im Projektpfad sollen keine Leerzeichen und keine Sonderzeichen sein. Außerdem soll die IDE wirklich über Gradle bauen. Das erkennt man daran, dass beim Starten Gradle-Ausgaben in der Konsole erscheinen.
