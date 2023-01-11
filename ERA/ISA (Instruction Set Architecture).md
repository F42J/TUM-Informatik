
Die ISA ist die zentrale Nutzer-Schnittstelle. Sie definiert z.B. welche Register, Datentypen, Adressierungsmodi, Speichermodell oder instructions ein Prozessor hat.  

Die ISA kann sich als Schicht unter dem Assemblercode und über der Binärrepräsentation vorgestellt werden.

Prozessoren mit der selben ISA sind Binärkompatibel. Aber die Geschwindigkeit kann unterschiedlich sein.

## Befehlssatz

Ist der Kern einer jeden ISA

### Befehlsklassen
- Arithmetische und logische Operationen
- Datentransfer
- Steuerung des Programmablaufs
Zusätzlich:
- Systembefehle für Verwaltungsaufgaben
- Ein-/Ausgabebefehle (bei manchen Architekturen): E/A-Geräte können auch mit eigenem Speicherbereich angesprochen werden. (Datentransferbefehle) 

### Ganzahlige Arithmetik

- Bsp: ADD, SUB, NEG, CMP (Vergleich), INC (Hochzählen), DEC (Herunterzählen). Ident für mit und ohne Vorzeichen
- MUL, DIV: Eine Variante für mit und ohne Vorzeichen. Ergebnis meist in zwei Registern:
	- Multiplikation: Doppelt so großes Ergebnis
	- Division: Ergebnis und Divisionsrest

- Bei ISA mit Statusregistern:
	Je nach Ergebnis werden einzelene Bits gesetzt Z(Null), C(Übertrag), V(Überlauf), N(Negativ)

### Gleitkomma Arithemtik

- Bsp: FADD, FSUB, FNEG, FABS (Absolutbetrag), FMUL, FDIV, FSQRT (Wurzel)
- Wird zwischen Gleitkomma und Ganzzahlen konvertiert
- Manchmal: Multiply-add-operation
	- Multiplikation und Addition (Subtraktion) in einer Operation
	- Auch bekannt als "Fused Multiply Add" FMA

### Logische Befehle

- Operanden sind Bitvektoren (1, 2, 3, 4, 5)
- Bitweises NOT, AND, OR, XOR

### Schiebe und Rotierbefehle

- Operanden sind Bitvektoren (1, 2, 3, 4, 5)
- Beispiel: Arithmetisches Rechtssschieben
- Beispiel: Linksrotieren über Carry Bit

### Sprungbefehle

Unbedingter Sprung:
 - Programm wird an anderer Stelle fortgesetzt.

Bedingter Sprung:
 - ISA mit Statusregister: Sprung wird abhängig von letzter arithmetischer Operation ausgeführt oder nicht
 - ISA ohne Statusregister: Arithmetische Operation z.B. CMP ist im selben Befehl
 - Für Verzweigungen (IF-ELSE) sowie Schleifen (FOR, WHILE)

Unterprogrammaufruf (CALL):
 - Vor dem Sprung: Rücksprungadresse wird auf den Stack gelegt
 - Spezieller Rücksprungbefehl (RET): Liest Rücksprungadresse aus dem [[Stack]]. (SP muss aber auf die Adresse zeigen)
 - Führ Methodenaufrufe gedacht

### Datentransferbefehle

LOAD/STORE bzw. MOVE:
- Transfer Speicher <-> Register

Optionen:
- Getrennte Speicherbefehle
- Unterschiedliche Befehle für Ganzzahl- und Gleitkommaregister