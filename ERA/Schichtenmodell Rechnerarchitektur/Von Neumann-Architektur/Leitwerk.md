Das Leitwerk steuert die [[Programmausführung]] des Codes. Dazu werden Befehle entsprechend der [[Befehlscodierung]] decodiert und dann die entsprechenden Befehle ausgeführt.

Das Leitwerk hat dabei eine direkte Anbindung an die [[ALU - Arithmetic Logic Unit|ALU]] für die Befehlsausführung arithmetischer Befehle sowie an den Speicher um die Befehle und die zugehörigen Daten zu laden (siehe [[Von Neumann Architektur|Zentraleinheit]]).

Zur Speicherung des Programmzustands beinhaltet das Leitwerk mehrere [[Register]]:
- **Befehslzähler(BZ bzw. PC)**: Der Befehszähler speichert die Adresse des aktuellen Befehls. Der Befehlszähler wird bei jeder Iteration des [[Maschinenbefehlszyklus]] erhöht und kann durch Sprünge beinflusst werden.
- **Instruktionsregister(IR)**: Zu Beginn jedes [[Maschinenbefehlszyklus]]wird der Befehl an der im PC gespeicherten Adresse in das IR geladen und dann [[Befehlscodierung|decodiert]] und ausgeführt.
- **Statusregister(SR)**:Die Statusregister speichern Informationen über die letzte Operation. Jeder Befehl beeinflusst dabei bestimmte Register, alle anderen Statusregister bleiben unverändert. 
   Welche Statusregister existieren unterschiedet sich je nach Architektur, mögliche Register sind:
   - 