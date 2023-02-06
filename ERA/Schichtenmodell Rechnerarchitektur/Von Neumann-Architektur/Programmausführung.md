Das von Neumann Prinzip macht folgende Aussagen zur Programmausführung:


### Leitwerk führt die Programmausführung durch

- Es wird immer nur ein einziger Befehl ausgeführt
- Befehlsadresse ist im Program-Counter (PC)
- Befehl wird ins Instruktionsregister (IR) geladen. Anschließend dekodiert und ausgeführt.
- Nach der Ausführung: 
	- Inkrementieren des PC und eventuell Sprung.

## Operationsprinzip

Die Befehlsabarbeitung durchläuft 2 Phasen. Dabei werden die [[Befehlscodierung|Befehle]] streng sequentiell abgearbeitet und passieren jeweils zuerst beide Phasen vor ein neuer Befehl bearbeitet wird.

### Interpretationsphase
Die im program counter (PC bzw. BZ) gespeicherte Adresse wird genutzt um den auszufühgrenden Befehl zu laden.

### Ausführungsphase

Durch die im Befehl enthaltene Adresse wird eine weitere Speicherzelle geladen und als Datenwert verarbeitet.




