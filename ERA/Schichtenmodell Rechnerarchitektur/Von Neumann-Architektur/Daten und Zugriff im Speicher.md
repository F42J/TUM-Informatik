

## Datenzugriff:

MAR und MDR.

MAR = Memory Access Register
MDR = Memory Data Register

Beim MAR wird die Adresse auf die Zugegriffen werden soll, angelegt. Beim MDR können dann die Daten ausgelesen werden.

## Adressierung

Der Speicher ist in der Praxis byte-adressierbar. D.h. die Adresse bezieht sich immer auf Bytegrenzen. 

Z.b. ![[Pasted image 20230109165317.png]]

Da Speicherzellen in mordernen Computern meist größer als 1 Byte sind sollten Daten entsprechend der Grenzen der Zellen ausgerichtet werden. 
Bei einer Zellengröße von n Byte wird ein Datum auf n Byte Grenzen ausgerichtet, die Startadressen einer Zelle sind also jeweils Vielfache von n. Damit gilt für die Startadresse mod n = 0.
Durch das Ausrichten der Daten auf Zellgrenzen(*alligned data*) können Speicherzugriffe minimiert werden 
Beispiel: bei 4-Byte Ausrichtung: Adresse 0, 4, 8, 12, 16, usw.

Es gibt auch sogennante "misaligned data". Die Daten sind dabei nicht ausgerichtet und überschreiten Zellengrenzen. Vorteil davon ist die effizientere Speichernutzung da kein "padding" notwendig ist. Nachteil ist mehr Speicherzugriffe und höherer Hardware-Aufwand.




