---
hide:
  - footer
---

## Importmöglichkeiten
Aktuell stehen zwei Möglichkeiten zur Verfügung, um Diplomify mit den nötigen Schüler- Lehrer - und Unterrichtsdaten zu versorgen: <br>

- [CSV-Import](#csv-import)<br>
- WebUntis-Import<br>

Welche Daten jeweils importiert werden können, zeigen die Tabellen. <br>


**Schüler*innen - Import**

| Merkmal Schüler*innen | CSV-Import                                                      | Webuntis-Import                             |
|-----------------------|:---------------------------------:|:-------------------------------------------:|
| Nachname              |:material-check-bold:{ .success }  |:material-check-bold: { .success }           |
| Vorname               |:material-check-bold:{ .success }  |:material-check-bold: { .success }           |
| Geburtsdatum          |:material-check-bold:{ .success }  |:material-check-bold: { .success }           |
| Geburtsort            |:material-check-bold:{ .success }  |nicht verfügbar { .danger }                  |
| Geschlecht            |:material-check-bold:{ .success }  |:material-check-bold: { .success }           |
| Aufnahmedatum         |:material-check-bold:{ .success }  |:material-check-bold: { .success }           |
| Klasse                |:material-check-bold:{ .success }  |:material-check-bold: { .success }           |
| Klasse-ID             |:material-check-bold:{ .success }  |:material-check-bold: { .success }           |
| Schüler-ID            |:material-check-bold:{ .success }  |:material-check-bold: { .success }           |

**Lehrer*innen - Import**

| Merkmal Lehrer*innen  | CSV-Import                        | Webuntis-Import                             |
|-----------------------|:---------------------------------:|:-------------------------------------------:|
| Nachname              |:material-check-bold:{ .success }  |:material-check-bold: { .success }           |
| Vorname               |:material-check-bold:{ .success }  |:material-check-bold: { .success }           |
| Benutzername          |:material-check-bold:{ .success }  |:material-check-bold: { .success }           |
| Klassenunterricht     |:material-close:{ .danger }        |:material-check-bold: { .success }           |
| Kursunterricht        |:material-close:{ .danger }        |:material-check-bold: { .success }           |
| E-Mail-Adresse        |:material-check-bold:{ .success }  |:material-check-bold: { .success }           |
| Schulverwaltungs-ID   |:material-check-bold:{ .success }  |:material-check-bold: { .success }           |

<br>

## CSV-Import

Die Quellen für die CSV-Dateien sind sehr schulindividuell, in der Regel können die Daten aber aus dem verwendeten Schulverwaltungsprogramm exportiert werden. <br>
Beim CSV-Import werden SuS automatisch ihren Klassen zugeordent. <br>
**Eine automatische Erstellung und Zuordnung zu Kursen (z.B. WPK oder Profile) erfolgt nicht.** <br>
Diese können aber leicht von den entsprechenden KuK angelegt werden.
<br>
### CSV-Schülerimport
**Vorbereitung**
!!! warning ""
    Die csv-Datei **muss** im Format UTF-8 formatiert sein und die Spalten müssen per **Semikolon** voneinander getrennt sein. <br>


 - [CSV-Datei aus DaNis exportieren...](Danisexport.md) <br>
    Beispiel [ansehen](../../img/01_Administration/schueler_csv_beispiel.png) oder [herunterladen](../../files/schueler_csv_beispiel.csv)

**Durchführung**

!!! bread ""
    Administrationsbereich > Imports | Schüler

1. Zuerst muss das Schuljahr ausgewählt werden, in das die SuS importiert werden sollen. Es ist wichtig, dass hier das korrekte Halbjahr ausgewählt ist.
2. Anschließend kann die DaNis-Exportdatei einfach auf das Datei-Auswahlfeld gezogen werden. Oder Sie klicken auf "Keine ausgewählt", um die Datei auf dem Computer zu suchen.
3. "Nächster Schritt"
4. Nun wird die Import-Datei gelesen und die Inhalte angezeigt. Hier können nun einzelne Schüler/innen abgewählt werden.
5. Wenn alle Voreinstellungen vorgenommen wurden, geht's weiter auf der Kontrollseite.
6. Hier können noch einmal alle Informationen geprüft werden. 
7. Ein Klick auf "Importieren" startet den Import.

!!! note ""
    Keine Sorge! Vor jedem Import wird automatisch ein Backup angelegt. Sollte etwas schiefgehen, kann jederzeit der vorherige Systemstatus wiederhergestellt werden.

<br>
### CSV-Lehrerimport (Vorbereitung)
Die CSV-Datei für den Schülerimport **muss** folgende Spalten enthalten (Andernfalls wird der Import abgebrochen. Zusätzliche Spalten werden ignoriert): 
!!! box ""
    - **Nachname**
    - **Vorname**
    - **Account** (wird als Benutzername verwendet)
    - **Import-ID** (eindeutige Zuordnung bei namensgleichen KuK)
    - **Email-Adresse** (Passworterstellung, 2-Faktor-Authentifizierung)


    <div class="danger">
        Lehrerbenutzer **müssen** eine Email-Adresse besitzen. <br><br>
        - Einladungsmail zur Passworterstellung kann nicht versendet werden <br>
        - Passwort kann nicht zurückgesetzt werden <br>
        - 2-Faktor-Authentifizierung per Mail kann nicht durchgeführt werden <br><br>
        Lehrerbenutzer ohne Email-Adresse werden nicht importiert.
    </div>

!!! warning ""
    Die csv-Datei **muss** im Format UTF-8 formatiert sein und die Spalten müssen per **Semikolon** voneinander getrennt sein. <br>
    
    **Beispiel [ansehen](../../img/01_Administration/lehrer_csv_beispiel.png) oder [herunterladen](../../files/lehrer_csv.csv)**


!!! success ""
    Eine Datei mit diesen Eigenschaften **[kann mit IServ](../../img/01_Administration/lehrer_iserv.gif)** erstellt werden. <br><br>
    In der exportierten Datei sollten nun einfach alle irrelevanten Spalten gelöscht werden.<br><br>
    Anschließend kann der Import in Diplomify erfolgen.
    
**Durchführung**
!!! bread ""
    Administrationsbereich > Imports | Lehrer

1. Die Importdatei kann einfach auf das Datei-Auswahlfeld gezogen werden. Oder Sie klicken auf "Keine ausgewählt", um die Datei auf dem Computer zu suchen.
2. "Nächster Schritt"
3. Nun wird die Import-Datei gelesen und die Inhalte angezeigt. Hier können nun einzelne Lehrkräfte abgewählt werden. Bitte achten Sie darauf, dass wirklich nur jene Lehrkräfte importiert werden, die tatsächlich Zugriff auf Diplomify haben dürfen. Vermeiden Sie auch Dummy-Daten, das hilft, die Datenbank "sauber" zu halten.
4. Wenn alle Voreinstellungen vorgenommen wurden, geht's weiter auf der Kontrollseite.
5. Hier können noch einmal alle Informationen geprüft werden. 
6. Ein Klick auf "Importieren" startet den Import.

!!! note ""
    Keine Sorge! Vor jedem Import wird automatisch ein Backup angelegt. Sollte etwas schiefgehen, kann jederzeit der vorherige Systemstatus wiederhergestellt werden.

!!! warning ""
    Beachten Sie, dass Diplomify nach dem Import automatisch Einladungsmails an alle neu importierten Lehrkräfte versendet. 
<br>

## WebUntis-Import
... Der Artikel wird gerade überarbeitet ...


