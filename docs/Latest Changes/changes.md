---
hide:
  - footer
  - navigation
  - toc
---


!!! box ""

	##17.12.2023

	###Import
	*	Import-Seite erlaubt jetzt Reload während Import (vorher Fehler-404)
	*	WebUntis-Import überarbeitet (Zugriff auf Timetable-API)

	###Zeugnisse
	*	Zeugnisanpassungen an Erlass zum Januar 2024
	*	Zeugnisse können kombiniert werden (z. B. Notenzeugnis + Anhang) [(mehr Infos...)](../Anleitungen/Administration/Zeugnisse_bearbeiten.md#3-zeugnisse-kombinieren)
	*	HTML der Zeugnisdateien kann direkt online editiert werden [(mehr Infos...)](../Anleitungen/Administration/Zeugnisse_bearbeiten.md#4-schnell-anderungen-am-template)
	*	Zeugnistemplates können mit Beschreibungen/Nachrichten für die Klassenlehrkräfte versehen werden [(mehr Infos...)](../Anleitungen/Administration/Zeugnisse_bearbeiten.md#2-informationen-fur-lehrkrafte-hinterlegen)

	###Zeugniskonferenzen
	*	Zeugniskonferenzen können nur noch von Klassenleitungen oder Admins gestartet werden [(mehr Infos...)](../Anleitungen/Schritt_für_Schritt/Zeugniskonferenz.md#1-konferenzstart)
	*	Zuschauermodus für Konferenzen [(mehr Infos...)](../Anleitungen/Schritt_für_Schritt/Zeugniskonferenz.md#3-zuschauermodus)

	### Zugriffsrechte/Sicherheit
	*	umfangreiche Vergabe von Schreib- und Leserechten durch den Admin
	*	Admins können Eingabezeiträume festlegen
	*	Klassenleitungsanträge können vom Admin bestätigt/abgelehnt werden
	*	Halbjahre sperrbar
	*	Klassenleitungen können Rechte für Co-Klassenleitungen und ILE-Berechtigte anlegen
	*	2-Faktor Authentifizierung über Authenticator-App oder e-Mail

	###diverse Verbesserungen in UI und Stabilität
	*	ILE-Bewertungen haben nun einen eigenen Bereich in der Klassenübersicht
	*	Klick auf den Schülernamen führt nun überall zur Schülereinzelansicht
	*	In der Schülereinzelansicht kann nun durch die gesamte Klasse geskippt werden
	*	Av/Sv Bemerkungen der Klassenleitung werden in der Einzelfachansicht angezeigt
	*	Auto-Save bei Noten- und Texteingaben ausgeweitet und mit Indikator versehen
	*	Fächer können Faktoren für die Durchschnittsberechnung erhalten
	*	Notentabelle kann nun von Noten- in Berichtsmodus geschaltet werden
	*	"Unterricht anlegen" komplett redesigned (Workflow optimiert, Mehrfachzuweisungen ausgeschlossen)
	*	Benutzername wird präsenter in der Willkommens-/Rücksetzungsmail angezeigt
	*	Ist ein/e Schüler/in zwei Unterrichten mit der gleichen Zeugnisentsprechung zugeordnet, wird die vergebene Bewertung auf dem Zeugnis angezeigt. Sind beide Unterrichte bewertet, wird die Bewertung des Unterrichts mit der höheren Priorität angezeigt. 
	<br>
	<br>



!!! box ""

	##17.06.2023 - Hot Requests

	*	Filter für Floskelkategorien
	*	Warnung, falls Lehrkräfte ohne Klassenleitungsstatus in der Klassenübersicht Av/Sv eintragen - statt in ihrem eigenen Unterricht.


!!! box ""

    ##04.05.2023    

	###Zeugnis & Konferenz
    *	Zeugnis-Basistemplates optimiert: effizientere (schnellere) Zeugniserstellung & Layoutverbesserungen
	*	Bemerkungsfelder können über beliebig viele Seiten wachsen.
	*	Komplett neue Konferenzansicht für Berichtszeugnisse.
	*	Der Versetzungsstatus steht standardmäßig auf „versetzt“.
	*	Notenhistorie in der Konferenzansicht.
	*	Farbliche Markierung der Noten in Konferenzansicht.
	* 	Notendurchschnitt in der Konferenzansicht.

	###Klassenübersicht
	*	Benutzte Floskeln erhalten jetzt für 10 Sekunden einen Indikator, damit Nutzer sicher sein können, dass die Floskel hinzugefügt wurde.
	*	Bei den Bemerkungen zu jedem Schüler können nun Notizen hinterlegt werden, die in der Zeugniskonferenz angezeigt werden.
	*	Smart-Floskel “Versetzung ist gefährdet“ erlaubt schnelles Hinzufügen von Versetzungsbemerkungen im 2. Hj.
	*	In der Fehltag-Tabelle lässt sich logischer mit Tab navigieren (Fehltage Schüler 1 > unentschuldigt Schüler 1 > Fehltage Schüler 2 > unentschuldigt Schüler 2 > usw.)
	*	"Konferenz starten" jetzt an präsenterer Stelle leichter zu finden.

	###Notentabelle
	*	Fächer, die nur im ersten Halbjahr unterrichtet wurden, werden in der Bewertungstabelle angezeigt.

	###Adminbereich
	*	Die Unterrichtstabelle erlaubt nun das Entfernen von hinzugefügtem Unterricht (im Adminbereich).
	*	Bezeichnung für Bemerkungsfelder ist schulindividuell einstellbar.
	*	Neue Ansicht „Berichte“ im Adminbereich. Das ist nun der Anlaufpunkt für Druckaufträge durch den Admin.
	*	Berichte über Anzahl und Art der vergebenen Abschlüsse.
	*	Statistik über versetzt, nicht versetzt und aufgerückt.
	*	Floskeln können nun mit geschlechtsabhängigen Formulierungen versehen werden: männlich|weiblich|divers < alle Angaben nötig.
	*	Bereits angelegte Floskeln sind jetzt editierbar.
	*	Fächern können nun Hilfstexte beigefügt werden, um die Kolleg*innen bei der Kurserstellung zu unterstützen.

	###Diverses
	*	Im Nutzerbereich ist nun eine Schülersuche, die direkt zur Schüler-Einzelansicht führt.
	*	diverse Verbesserungen in UI und Stabilität

	###Technisches
	*	Im Hintergrund überwacht nun ein Masterserver alle Diplomify Instanzen und meldet Auslastungsspitzen, heruntergefahrene Server oder andere Probleme.
	*	Ein neues Server-Verwaltungssystem erlaubt uns nun das flexible Erstellen oder Leistungsanpassungen bei vorhandenen Servern, sollte der Masterserver Leistungsprobleme melden. - Dabei läuft jede Instanz weiterhin auf dedizierten Servern in Deutschland.
	<br>
	<br>
