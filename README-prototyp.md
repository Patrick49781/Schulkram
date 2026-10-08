# Teilelotse: Prototyp, Stand 8. Oktober 2026

Eine Datei: `herstellerxy-website.html`, rund 125 KB. Doppelklick genügt, läuft offline, braucht keinen Server und keine Installation. Auf dem Telefon testen, nicht am Laptop: dafür ist er gebaut.

## Was das hier ist

Die Website eines erfundenen Maschinenbauers, **HerstellerXY GmbH** aus Schwäbisch Gmünd, mit dem Ersatzteilportal als Teil davon. Der Prototyp zeigt, wie das Portal unter der Marke eines Herstellers aussieht und wie ein Instandhalter damit bestellt. Er ist für Nutzergespräche gemacht und wird danach weggeworfen, es ist kein Vorläufer des späteren Produkts.

Einstieg über den Knopf "Ersatzteile" im Menü. Dort liegen vier Typenschilder zum Antippen.

## Was echt funktioniert

- Teileliste genau einer Maschine, 264 Teile über drei Baureihen
- Suche über Benennung und Teilenummer, Filter nach sechs Baugruppen und nach Verschleißteilen
- Block "Häufig gebraucht an dieser Maschine" über der vollständigen Liste
- Warenkorb über mehrere Maschinen hinweg, Mengen in Verpackungseinheiten
- Bestellformular ohne Konto, mit Pflichtfeldprüfung, Bestellnummer HXY-2026-0001 aufsteigend
- Eilbestellung "Maschine steht" mit 3 Prozent Zuschlag, rechnet live mit
- Sicht des Innendienstes auf alle Vorgänge, mit Kennzahlen und ERP-Datensatz
- Postausgang mit beiden Mailtexten und dem strukturierten Anhang
- Etikettenbogen mit QR-Codes, druckbar im 24er-Raster

## Was angetäuscht ist

| Im echten Produkt | Im Prototyp |
|---|---|
| Datenimport vom Hersteller | Daten stecken fest in der Datei |
| Mailversand | Postausgang im Browser, es geht nichts raus |
| ERP-Anbindung, echte Bestände | nur Kennzeichen Lagerteil oder Beschaffungsteil |
| Bilder je Teil | stilisierte Piktogramme je Teilegruppe |
| Anmeldung im internen Bereich | ohne Anmeldung erreichbar |

**Der QR-Scan funktioniert noch nicht.** Die Codes zeigen auf `teile.herstellerxy.de`, eine erfundene Adresse. Format und Inhalt stimmen (eine URL nach IEC 61406), nur gehostet ist nichts. Im Gespräch also antippen statt scannen.

## Die vier Maschinen und wofür sie da sind

| Maschine | Zweck im Gespräch |
|---|---|
| HXY-2016-0471, Kantenschleifer | einfacher Fall, 38 Positionen |
| HXY-2021-1180, Doppelschleifer | 214 Positionen, hier zeigt sich, ob Suche und Filter tragen |
| HXY-2023-0455, Doppelschleifer | 2024 umgebaut, Teile der Steuerung "kann abweichen", enthält ein abgekündigtes Teil mit Nachfolger |
| HXY-2009-0112, Handschleifer | **keine geprüfte Stückliste**, nur Typliste, Bestellen gesperrt, stattdessen Anfrage |

Die letzte Maschine ist der wichtigste Fall. In echten Herstellerdaten wird er häufig sein, und genau daran entscheidet sich, ob das Produkt trägt.

Weitere Fälle, verstreut in der Liste: 93 Teile mit Verpackungseinheit (Packung zu 10, Satz zu 4), 23 Zukaufteile von Fremdfabrikaten, die nicht über den Hersteller bestellbar sind.

## Zahlen sind erfunden

Preise, Teilenummern, Maschinennummern, Firmengeschichte, 4.212 Maschinen im Feld: alles ausgedacht. Die Preise liegen in plausiblen Bändern je Teilegruppe, damit im Gespräch niemand über 1.200 Euro für einen Dichtring stolpert, aber sie sind nicht recherchiert.

## Zwei Dinge für die Auswertung

**Protokoll.** Interner Bereich, Punkt "Protokoll dieses Gesprächs": Zeit bis zur ersten Suche, Suchen ohne Treffer, hinzugefügte Teile, Verlauf. Läuft nur im Browser, nach jedem Gespräch ablesen und leeren.

**Datenherkunft.** Interner Bereich, Punkt "Woher die Daten kommen": die zwei CSV-Dateien, die der Hersteller liefern müsste, mit Pflichtspalten und den Folgen fehlender Spalten. Das ist die Seite für das Gespräch mit dem Serviceleiter.

## Zurücksetzen

Der Zustand liegt in der Sitzung des Browsers. Tab schließen, neu öffnen, alles ist leer. Zwischen zwei Gesprächspartnern also einfach den Tab neu starten.
