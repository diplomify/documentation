---
hide:
  - footer
---

!!! danger ""
    Die Merkmale müssen sämtlich vorhanden sein und genau so benannt, wie angegeben.<br>
    Alle Merkmale müssen Daten enthalten.

<br>
## Exportdatei erstellen
**Die Anleitung bezieht sich auf DaNis in der Version 3**

### 1.: Exportmenü öffnen

Öffne DaNis und wähle im Menü „Berichte“ „Freie Liste“ aus.

![Bewertungstabelle](../../img/01_Administration/Danisexport_1.png){ .image-75 } 

### 2. Exporteinstellungen vornehmen

Markiere im linken Feld folgende Merkmale: <br>

!!! box ""
    - **SchuelerNachname**
    - **SchuelerRufname**
    - **SchuelerGeburtsdatum** (für das Geburtsdatum auf dem Zeugnis)
    - **SchuelerGeburtsort** (für den Geburtsort auf dem Zeugnis)
    - **SchuelerAufnahmedatum** (wird aus Abgangszeugnissen angegeben)
    - **SchuelerGeschlecht** (für gendergerechte Floskeln)
    - **GruppeBezeichnung** (Klassenangabe auf dem Zeugnis und Zuordnung zur Klasse)
    - **GruppeId** (eindeutige Identifikationsnummer der Klasse bei Mehrfachimporten)
    - **SchuelerId** (eindeutige Identifiktaionsnummer des Schülers bei namensgleichen Schülern)

Wähle anschließend im Bereich „Schulgliederungsauswahl“ das Schuljahr aus, das importiert
werden soll. (In der Regel das aktuelle.) <br>
Im Bereich „Gruppenauswahl“ wähle „Alle Gruppen“, um die gesamte Schülerschaft und alle Klassen zu exportieren.

![Bewertungstabelle](../../img/01_Administration/Danisexport_2.png){ .image-75 }

### 3. Auswahl für später speichern

Speichere die Merkmalauswahl, damit du beim nächsten Export sofort darauf zugreifen kannst.
Klicke dazu auf das kleine grüne Häkchen im Bereich „Feldauswahl“ und vergib bspw. die Bezeichnung „Diplomify - Schülerexport“.

### 4. CSV-Datei erstellen

Nun kann die Exportdatei erstellt werden:
Klicke dazu rechts auf CSV-Export.
Bei der anschließenden Abfrage kannst du festlegen in welchem Format die Datei erstellt werden soll. **Wähle bitte unbedingt UTF-8.**

!!! danger ""
    Die Datei darf nicht "gekürzt" werden. <br>
    Wenn nur ein Kind verändert werden soll, muss trotzdem mindestens die ganze Klasse des Kindes importiert werden.<br><br>
    Bei einem Import aktualisiert Diplomify die Klassenlisten. Wenn ein Kind die Klasse wechselt, wird es in der neuen Klasse eingetragen und aus der alten entfernt. Das kann dazu führen, dass andere Kinder fälschlicherweise gelöscht werden, wenn sie nicht in der Importdatei stehen. Zudem werden die Bewertungen des Kindes zurückgesetzt, da es jetzt von anderen Lehrkräften bewertet wird.

    Bitte daher immer die gesamte Klasse in der Importdatei aufführen. Ein direkter Import des kompletten Exports von Danis ist am besten. Individuelle Änderungen können in Diplomify gemacht werden, aber neue Schüler sollten dort nicht angelegt werden, da diese keine Import-ID erhalten. - Was beim nächsten Import zu Zuweisungsproblemen führt.

<hr>

Die erstellte Datei kann nun in Diplomify importiert werden. <br>
[Zum Artikel über den Import...](../Administration/Import.md)
