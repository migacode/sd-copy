# SD-Copy - Simple Disk Copy
Einfaches Front-End Script für <b>ocs-onthefly</b> (Clonezilla) und <b>dd</b> zum Kopieren bzw. Klonen von beliebigen Speichermedien wie SD-Karten, USB-Sticks, Festplatten etc.<br />
Wem die Bedienung von Clonezilla zu aufwendig ist, der kann einen Kopiervorgang mit diesem Tool sehr viel einfacher erledigen. Alle angeschlossenen Laufwerke werden nach dem Start des Skriptes direkt angezeigt und können sofort einfach mit ihrem durch das Betriebssystems zugeordneten "Buchstaben" ausgewählt werden.<br />
Alternativ dazu gibt es einen interaktiven Modus, bei welchem man nacheinander das Quell- und Ziel-Laufwerk anschließen kann und <b>SD-Copy</b> diese dabei automatisch erkennt und auswählt.<br />
Bei dem Kopiervorgang werden dann wahlweise nur die belegten oder alle Sektoren des Speichermediums kopiert, wobei die erste Option erheblich Zeit spart.<br />
Darüber hinaus wird auch immer der erste Sektor des Speichermediums mit dem Bootloader (MBR) kopiert, so dass dieser auf der Kopie nicht mehr nachträglich mit externen Tools korrigiert werden muss.<br />
Zudem ist es auch möglich, nur den Bootloader alleine zu kopieren, was bei der Reparatur nicht mehr startfähiger Systeme hilfreich sein kann.<br />
<br />
(Nach dem Download "<b>chmod a+x</b>" nicht vergessen ;)
<br />
<br />
<b>Optionen zum Aufruf per Kommandozeile:</b><br />
<code>
  -a, --automode  Startet immer direkt den automatischen Modus.<br />
  -b, --bootonly  Kopiert nur den Bootsektor (MBR) und keine sonstigen Daten.<br />
  -d, --deep      Setzt den Deep-Modus (dd) als Vorgabe für den Kopiermodus.<br />
  -h, --help      Zeigt die Hilfe an.<br />
  -n, --noupdate  Sucht nicht nach Updates für dieses Skript.<br />
</code>
<hr>
<br />
Sämtliche Software auf diesen Seiten wird ohne Mängelgewähr und ohne jegliche ausdrückliche oder stillschweigende Garantie zur Verfügung gestellt, einschließlich und ohne Einschränkung jeglicher Garantie für die Gebrauchstauglichkeit oder Eignung für einen bestimmten Zweck. Alle Risiken in Bezug auf Ergebnisse und Leistung dieser Software werden vollständig vom Benutzer übernommen!
