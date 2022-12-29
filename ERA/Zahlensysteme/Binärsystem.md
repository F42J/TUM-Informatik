Das Binärsystem benutzt die Basis 2, als Zahlsymbole sind also 1 und 0 möglich. Das System basiert wie das Dezimalsystem auf Potenzen für die Weertigkeit der Ziffern, es kann also die [[Allgemeine Formel für Zahlensysteme]] verwendet werden.

Vorteil des Binärsystems ist, dass es sich sehr gut durch 2 Zustände *Strom* und *kein Strom* in elektrischen Schaltungen darstellen lässt.

Ein großer Nachteil des Systems ist, dass große Zahlen schnell sehr unübersichtlich wird, weswegen zur Darstellung für Menschen häufig das [[Hexadezimalsystem]] benutzt wird.

**Arithmetik** im Binärsystem funktioniert wie im Dezimalsystem. Anbei sind Beispiele für die 4 Grundrechenarten:

**Addition**
![[addition_binaer.png]]
*Step-by-step guide:*
1. Schreibe beide Zahlen rechtsbündig auf und fülle sie links mit 0en auf
2. Lasse eine weitere Zeile frei für den Übertrag
3. Starte beim rechtesten Ziffernpaar.
4. Addiere die beiden Ziffern und den Übertrag  zusammen
5. Sollte das Ergebnis größer werden als die Basis des Zahlensystems (hier 2), notiere bei der nächsten Stelle in der Zeile Übertrag eine 1.
6. Notiere das Ergebnis der Addition modulo der Basis (d.h wird die Basis überschritten fängt man wieder von 0 an z.B. 9+7= 16, es wird 10 überschritten und dann wieder von 0 bis 6 hochgezählt, das Ergebnis der Stelle ist also 6)
7. Wiederhole die Schritte ab 4. für alle weiteren Ziffern
8. Schreibe den evtl verbliebenen Übertrag als neueste linke Stelle auf


**Subtraktion** 
![[subtraktion_binaer.png]]
*Step-by-step guide:*
1. Schreibe beide Zahlen rechtsbündig auf und fülle sie links mit 0en auf
2. Lasse eine weitere Zeile frei für den Übertrag
3. Starte beim rechtesten Ziffernpaar.
4. Subtrahiere die die zweite Ziffer und den Übertrag von der ersten Ziffer
5. Sollte das Ergebniskleiner als 0 werden, notiere bei der nächsten Stelle in der Zeile Übertrag eine 1.
6. Notiere das Ergebnis der Subtraktion als Ergebnis der Ziffer. Wird das Ergebnis kleiner als 0 wird wieder von der Basis (hier 2) gestartet und der Rest abgezogen
7. Wiederhole die Schritte ab 4. für alle weiteren Ziffern
