
Der Stack ist eine Datenstruktur nach dem Lifo-Prinzip (Last in, first out).

Es gibt zwei wichtige Operationen:

- PUSH: Legt einen Wert oben auf den Stack drauf.
- POP: Nimmt den obersten Wert auf dem Stack gibt ihn zurück und entfernt ihn vom Stack.

Der SP (ESP, RSP) ist der Stack Pointer. Er zeigt immer auf den obersten Wert am Stack.

Der BP (EBP, RBP) ist der Base Pointer. Er zeigt auf den obersten Wert am Stack *zum Zeitpunkt an dem das momentane Unterprogramm aufgerufen wurde*.
Sprich meistens auf die Rücksprungadresse zum vorherigen Unterprogramm.  

Der Bereich zwischen BP und SP wird auch Stack Frame gennant.

*Der Stack wächst nach unten, sprich von der größten Adresse in Richtung zur kleinsten.*