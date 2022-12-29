Festkommazahlen teilen den Speicher in 2 Bereiche für Vor und Nach dem Komma. Das kann dann beispielsweise wie folgt aussehen:

![[festkommazahl_beispiel.png]]
In dem Beispiel wäre die Zahl ist 2,5625. Dabei wird die 2 durch die ersten 4 Bit(grün markiert) dargestellt. Die letzten 4 Bit(rot markiert) stellen dann die ,5625 dar.

Zur Berechnung des Wertes einer Festkommazahl kann die [[Allgemeine Formel für Zahlensysteme]] verwendet werden und auf negative Indizes erweitert werden. Damit hat also das erste Bit vor dem Komma die Position 0, die Bits für die Nachkommastellen werden von der 0 asugehen nach rechts mit negativen Indizes durchnummeriert. Das heißt die erste Ziffer nach dem Komma hat den Index -1 und wird entsprechend auch mit ^(-1) berechnet, die zweite Ziffer nach dem Komma analog -2 etc.

Die [[Festkommaarithmetik]] funktioniert grundlegend wie die normale Arithmetik im [[Binärsystem]], jedoch müssen einige Aspekte bei der Position des Kommas beachtet werden.