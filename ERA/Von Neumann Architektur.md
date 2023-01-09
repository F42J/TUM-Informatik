
- Rechnerstruktur unabhängig vom bearbeiteten Problem
- Programm und Daten im gleichen Speicher
- Speicher ist in Zellen gleicher größen unterteilt, die durch fortlaufende Nummern (Adressen) bezeichnet werden.
- Programm ist eine Reihe von Befehlen (aufsteigende Adressen, Sequentiell)
- Zahlen werden dual dargestellt.
- Von der Folge kann durch bedingte oder unbedingte Sprünge abgewichen werden.


### Rechner besteht aus 4 Werken:

- Haupt- bzw. Arbeitsspeicher (Programme und Daten)
- Leitwerk (interpretiert Programme)
- Rechenwerk (arithmetische Operationen)
- Ein-/Ausgabewerk inklusive Sekundärspeicher (kommuniziert mit peripherie Geräten bzw. Umgebung)

## Speicher:

- Ist in Zellen gleicher größe unterteilt. (Gängige Größen Double Word (32bit) oder Quad Word (64bit))
- Jede Zelle hat eine Adresse und jede Zelle einen Wert.

## Programmablauf:

Befehler werden immer sequentiell ausgeführt und in aufsteigender Adressreihenfolge gespeichert. Abweichung ist durch Sprünge möglich.

### Leitwerk führt die Programmausführung durch

- Es wird immer nur ein einziger Befehl ausgeführt
- Befehlsadresse ist im Program-Counter (PC)
- Befehl wird ins Instruktionsregister (IR) geladen. Anschließend dekodiert und ausgeführt.
- Nach der Ausführung: 
	- Inkrementieren des PC und eventuell Sprung.

## Operationsprinzip

Der Befehlsablauf ist sequentiell und streng seriell

### Interpretationsphase
 Durch PC wird Inhalt einer Speicherzähle geholt (Adresse des Befehls). Die Adresse wird dann als Befehl interpretiert.

### Ausführungsphase

Durch die im Befehl enthaltene Adresse wird eine weitere Speicherzelle geholt und als Datenwert verarbeitet.


## Bildliche Darstellung
![[Pasted image 20230109172211.png]]

## Zentraleinheit

Zentraleinheit (ZE) = 
- Leitwerk
- Rechenwerk
- Speicher

Die Einheit arbeitet im [[Maschinenbefehlszyklus]] = Interpretationsschleife

Beschreibt den Rechner und seine Funktionsweise auf unterem Abstratktionsniveau: 
- Maschinenbefehls- bzw. Register-Transfer-Ebene (Register-Transfer-Level (RTL))