Ein Befehl wird grundsätzlich aus 2 Teilen aufgebaut, dem **Opcode**, der angibt welcher Befehl ausgeführt werden soll, und den **Operanden** , die Parameter für den Befehl beinhalten.

Dabei können die Befehle auf 2 Arten codiert werden:
- Einheitliches Format:
	- feste Länge
	- leichtes dekodieren
	- üblich bei [[RISC vs. CISC|RISC]] ISAs
	- kein Platz für Adresssen
	- unflexibel
- Variables Befehlsformat
	- flexibel
	- alle Adressierungsarten für alle Operanden zugelassen
	- decodieren zeitaufwändig
	- Probleme bei Speicherverwaltung