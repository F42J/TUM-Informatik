
## Überdeckte Adressierung, Implizit, Explizit

Zieladresse ist identisch mit einer der Quelladressen. Ein Operand wird quasi überschrieben.

Implizit: Adresse ist fest vorgegeben
Explizit: Adresse wird im Befehl angegeben (benötigt Speicher, muss dekodiert werden)

## Nulladressform

Adressen werden nicht explizit angegeben.

Z.b. Operanden sind die obersten Elemente im Stack und das Ergebnis wird wieder auf den Stack gelegt.

Beispiel: Lua-Stack (i love it), JVM, IA-32 Gleitkommabefehle

*Kellermaschine*

## Einadressform

Ein Operand ist immer dasseble Register (z.B. Akkumulator) und das Ergebnis wird wieder dort abgelegt.

Bsp: AC + x wird in AC abgelegt.

[[Von Neumann Architektur]], Frühe 8-Bit Prozessoren

Nachteil: Unflexibel, Häufiges Laden des AC

## Zweiadressform

Ergebnis überschreibt den ersten Operanden. Gleich wie Einadressform nur das das Register (dort AC) explizit angegeben werden kann. Aber: Ein Operand muss ein Register sein => nur ein Operand kann im Hauptspeicher stehen.

Beispiel: IA-32, Registermaschine

## Dreiadressform

Operanden und Ergebnis werden explizit adressiert. x + y = z Wobei x, y, und z alles Register sind.  => Register-Register-Modell (RISC-CPUs)
oder Speicher-Speicher-Modell wenn Operanden + Ergebnis im Hauptspeicher stehen können. (Frühe CISC-CPUs) siehe [[RISC vs. CISC]]

Nachteil: Befehl benötigt viel Speicherplatz und viele Speicherzugriffe


