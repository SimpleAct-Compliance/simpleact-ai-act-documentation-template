# Die Nachweisschicht

Die technische Dokumentation ist kein Nachweis. Sie ist eine **Beschreibung**, die auf Nachweise verweist. Wer das verwechselt, schreibt ein Dokument, das Behauptungen über sich selbst aufstellt.

## Der Unterschied

| | Dokumentation | Nachweis |
|---|---|---|
| sagt | so ist das System gebaut | so wurde es belegt |
| Form | Text, Diagramme, Tabellen | Protokoll, Messung, Vertrag, Aufnahme |
| Urheber | wer dokumentiert | wer gemessen, geprüft, unterzeichnet hat |
| Prüfung fragt | ist es beschrieben? | können Sie es zeigen? |

Beispiel: Der Satz „das System erreicht eine Genauigkeit von 94 % auf dem Validierungsdatensatz" ist Dokumentation. Das Testprotokoll mit Datum, Datensatz-Kennung, Metrik und Ergebnis ist der Nachweis. Ohne das Protokoll ist der Satz eine Zahl, die jemand aufgeschrieben hat.

## Was ein Nachweis mindestens trägt

| Bestandteil | Ohne es |
|---|---|
| **Version** des Systems | belegt er einen Zeitpunkt, nicht einen Zustand |
| Datum | ist nicht feststellbar, was wann galt |
| Fundort | ist er nicht vorlegbar |
| Urheber | gibt es keinen Ansprechpartner |
| Bezug zum Abschnitt | weiß niemand, was er belegt |

Die letzte Zeile wird unterschätzt. Ein Ordner mit vierzig Dateien, von denen niemand sagen kann, welcher Anhang-IV-Abschnitt welche braucht, ist in einer Prüfung ein Ordner mit vierzig Dateien.

## Welcher Abschnitt welchen Nachweis braucht

| Anhang-IV-Abschnitt | Nachweisart |
|---|---|
| allgemeine Beschreibung, Version | Release-Notes, Versionsstand im System |
| Entwurfsentscheidungen | Entscheidungsprotokoll mit Datum |
| Datenanforderungen | Datenquellentabelle, Rechtsgrundlage, Bereinigungsprotokoll |
| menschliche Aufsicht | **Nutzungskennzahl**: wie viele Ausgaben wurden geändert |
| Validierung und Test | Testprotokoll je Version, datiert |
| Genauigkeit, Robustheit, Cybersicherheit | Messwerte mit Datensatz-Kennung; Prüfbericht |
| Risikomanagement | Risikoregister mit Bewertung und Maßnahmen |
| Änderungen | Änderungstabelle, verknüpft mit Releases |
| Normen | Normverweis mit Fassung |
| Konformitätserklärung | unterzeichnete Erklärung mit Datum |

Zur vierten Zeile: Der Nachweis für **menschliche Aufsicht** ist der am schwersten zu beschaffende und der aussagekräftigste. Die Dokumentation kann beschreiben, dass Aufsicht technisch ermöglicht wird. Dass sie tatsächlich ausgeübt wird, belegt nur eine Zahl: wie viele Ausgaben im Betrieb geändert oder verworfen wurden.

## Reihen statt Einzelstücke

Für drei Dinge ist ein einzelner Nachweis strukturell ungeeignet, weil die Pflicht ein **Fortlaufen** verlangt:

| Gegenstand | Nachweis ist |
|---|---|
| Beobachtung nach dem Inverkehrbringen (Art. 72) | die Reihe der Berichte |
| Validierung über Versionen | die Reihe der Testprotokolle |
| Änderungen am Lebenszyklus | die vollständige Tabelle, nicht der letzte Eintrag |

Ein einzelner aktueller Bericht belegt hier nichts: Er kann am Vortag der Prüfung entstanden sein. Die Lücke in der Reihe ist dagegen aussagekräftig — und sie ist der Grund, warum ein halbes Jahr ohne Eintrag schwerer zu erklären ist als ein fehlender Abschnitt.

## Vier Zustände je Nachweis

**offen** (noch nicht erbracht, mit Person und Termin) → **erbracht** (liegt vor, niemand hat nachgesehen) → **geprüft** (eine zweite Person hat inhaltlich nachgesehen) → **freigegeben** (mit Versionsbezug bestätigt).

Und **zurück auf offen**, wenn eine neue Version läuft. Dieser Rückweg fehlt in vielen Ablagen: Der Nachweis bleibt freigegeben, während das System drei Versionen weiter ist.

Ausführlich zu den Zuständen: [Prüfliste AI Act](https://github.com/SimpleAct-Compliance/simpleact-ai-act-checklist)

## Wann ein Nachweis ungültig wird

| Ereignis | Betroffene Nachweise |
|---|---|
| neue Produktversion | alle mit Versionsbezug |
| Modellwechsel beim Anbieter einer Komponente | Genauigkeit, Robustheit, Verhalten |
| neue Datenquelle | Datenquellentabelle, Rechtsgrundlage |
| Änderung der Zweckbestimmung | **alles** — und die Rollenfrage neu |
| zuständige Person weg | Zuständigkeits- und Freigabenachweise |

Alte Nachweise werden nicht gelöscht. In einer Prüfung lautet die Frage, was zu einem bestimmten Zeitpunkt belegt war.

## Fremdbestandteile

Wer ein Modell oder eine Komponente eines Dritten verwendet, dokumentiert: welches, welche Version, welcher Anbieter — und **welche Angaben er liefert und welche nicht**.

Der zweite Teil ist der wichtigere. Ein Anbieter, der die Modellversion nicht herausgibt, erzeugt eine Lücke in Ihrer Dokumentation, die Sie nicht schließen können. Diese Lücke gehört benannt, mit Datum der Anfrage — dann ist sie ein Befund gegen den Anbieter und nicht gegen Sie.

Dazu: [Anbieterregister](https://github.com/SimpleAct-Compliance/simpleact-model-vendor-register)

## Lücken benennen

Ein Abschnitt mit „liegt nicht vor, verantwortlich ___, Termin ___" ist besser als einer mit Füllsätzen. Füllsätze fallen auf, und sie stellen den Rest in Frage: Wer einen Abschnitt erkennbar mit Worten gefüllt hat, hat möglicherweise mehrere so gefüllt.

Eine benannte Lücke zeigt dagegen, dass jemand den Abschnitt gelesen und verstanden hat.

## Weiter

[Was laufend entstehen muss](./documentation-logic.md) · [Dokumentationsprüfung](../../templates/documentation-checklist.md)
