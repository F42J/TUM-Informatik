Das Von-Neumann-Prinzip macht folgende Aussage über den Speicher
>  Speicher ist in Zellen gleicher Größen unterteilt, die durch fortlaufende Nummern (Adressen) bezeichnet werden.
>  Programm und Daten im gleichen Speicher

Aus diesem Prinzip folgen 2 grundlegende Aussagen:
- *gleich große Zellen*
  Der Speicher besteht aus beliebig vielen Zellen einer große. Diese Größe kann dabei 1 Byte sein, es sind aber auch andere Größen wie z.B ein word möglich ([[Gängige Wortlängen]])
- *fortlaufende Nummerierung*
   Alle Speicherzellen haben eine einheitliche fortlaufende Nummer, mit der die einzelnen Zellen addressiert werden können ([[Daten und Zugriff im Speicher]])
   
### Typische Speicherverwaltung

Jedes Programm hat einen Adressraum
- Enthält Daten und Programm
- Code ("text") wird meist am unteren Ende geladen.
- Statische Daten (Fest alloziert, Teil des Codes)
- Dynamische Speicherverwaltung (Heap): Kann angefragt und freigegeben werden. Wächst nach oben 


## moderner Von-Neumann Speicher

|**beibehalten** | **Neuerungen**| **Kritik** |
|---------|-------|----------|
|Speicherbreite variiert (ist aber meist statisch)|Segmentierung|Datentypinformation sollte zur Laufzeit mitgeführt werden|
|Ühysikalische Adresslänge kann von der Repräsentierung einer Adresse abweichen( 64 bit Adresse bei 40-48 Adressleitungen in modernen Computern)|Virtueller Speicher(Indirektion aller Adressen)|Benutzung von Variablen führt zu schwierig beweisbaren Eigenschaften|


### Bennenung Speichermengen


![[Pasted image 20230206163618.png]]






