

## Datenzugriff:

MAR und MDR.

MAR = Memory Access Register
MDR = Memory Data Register

Beim MAR wird die Adresse auf die Zugegriffen werden soll, angelegt. Beim MDR können dann die Daten ausgelesen werden.

## Adressierung

Der Speicher ist in der Praxis byte-adressierbar. D.h. die Adresse bezieht sich immer auf Bytegrenzen. 

Z.b. ![[Pasted image 20230109165317.png]]

Ein Datum kann auf eine n-Byte Grenze ausgerichtet sein. Damit ist die Adresse ein Vielfaches von n. Zum Beispiel bei 4-Byte Ausrichtung: Adresse 0, 4, 8, 12, 16, usw.
Damit gilt Adresse mod n = 0.

Häufig muss ein Datenformat der Größe s auf s-Byte Grenzen ausgerichtet sein. Dadurch können Speicherzugriffe minimiert werden.

(Wird auch "aligned data" gennant)

Es gibt auch sogennante "misaligned data". Die Daten sind nicht ausgerichtet. Vorteil davon ist die effizientere Speichernutzung da kein "padding" notwendig ist. Nachteil ist mehr Speicherzugriffe und höherer Hardware-Aufwand.