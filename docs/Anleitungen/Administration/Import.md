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

 - [CSV-Datei aus DaNis exportieren...](Danisexport.md) <br>
    Beispiel [ansehen](../../img/01_Administration/schueler_csv_beispiel.png) oder [herunterladen](../../files/schueler_csv_beispiel.csv)


<br>
### CSV-Lehrerimport (Vorbereitung)
Die CSV-Datei für den Schülerimport **muss** folgende Spalten enthalten: 
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
    
    **Beispiel [ansehen](../../img/01_Administration/lehrer_csv_beispiel.png) oder [herunterladen](../../files/lehrer_csv_beispiel.csv)**


!!! success ""
    Eine Datei mit diesen Eigenschaften [kann mit IServ](../../img/01_Administration/lehrer_iserv.gif) erstellt werden. (minimale Nachbearbeitung nötig)
    
<br>
## WebUntis-Import
... Der Artikel wird gerade überarbeitet ...


