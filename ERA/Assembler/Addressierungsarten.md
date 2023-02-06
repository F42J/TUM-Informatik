#### Adressierungsarten
Jeder Befehl spezifiziert die zu bearbeitenden Daten (in Form von Operanden). Das können Konstante Werte, Register, oder direkt Speicheradressen sein.

*Adressierung* = Spezifikation des Operanden
*Adressierungsart* = Methode zur Spezifikation (Merkmal der [[ISA (Instruction Set Architecture)]])

- Unimttelabre Adressierung = Konstanter Wert
- Register Adressierung = Operand steht im Register und der Registername steht im Befehl
- Speicheradressierung = der Operand steht im Hauptspeicher. Adresse wird an Befehl übergeben. Allerdings meist *nicht direkt* sondern wird erst berechnet *(Base + (Index * Scale) + Displacement = effektive Adresse)*

##### Dynamische Adressierung

Adresse wird zur Laufzeit berechnet. Kann aus Registern + Hauptspeicher zusammengebaut werden:  *(Base + (Index * Scale) + Displacement = effektive Adresse)*

Dadurch flexiblere Adressierung. Z.b. Iterieren über ein Array oder dynamische Datenstrukturen (List, Tree, etc.)

##### Direkte Adressierung

Adresse steht konstant im Befehl.

##### Registerindirekte Adressierung

Adresse steht in einem Register.

- *Prä/Postdekrement*:
   Adresse wird um 1,2,4 oder 8 verkleinert. (Schleifen, Stack)
- *Displacement (Basisrelative Adressierung)*: Ein Wert (positiv oder negativ) wird zur Adresse hinzuaddiert (Zugriff auf Felder mit festem index (*indizierte Adressierung*))
- *Skalierungsfaktor*:
   Gleich wie ein Displacement Faktor nur das dieser noch mit einem Wert multipliziert wird bevor er hinzuaddiert wird (index * scale)
- *Befehlszähler-relative Adressierung*:
   Adresse wird relativ zum Befehlszähler gebildet (siehe Displacement). Ermöglicht positions unabhängigen Code (PIC). (siehe Sprünge, Unterprogrammaufrufe, etc.)
- *Speicherindirekte Adressierung*:
   Adresse des Operanden steht im Speicher. Z.b. Variable die auf den Beginn einer Array zeigt.

Adressierungsarten erzeugen Komplexizität im Gegenzug zu einfacherer Programmierbarkeit => [[ISA (Instruction Set Architecture)]] Designentscheidung.