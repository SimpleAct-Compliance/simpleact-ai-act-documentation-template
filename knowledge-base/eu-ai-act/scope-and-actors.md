# Wer dokumentieren muss

Die technische Dokumentation nach **Art. 11 in Verbindung mit Anhang IV** ist eine **Anbieterpflicht** für Hochrisikosysteme. Das klingt nach einer klaren Abgrenzung und ist es nicht.

## Die Pflicht trifft den Anbieter

| Rolle | Anhang IV | Weitere Dokumentationspflichten |
|---|---|---|
| **Anbieter** | ja | Risikomanagement (Art. 9), Qualitätsmanagement (Art. 17), Konformitätserklärung, Registrierung |
| **Betreiber** | nein | Protokolle aufbewahren (Art. 26), ggf. Grundrechte-Folgenabschätzung (Art. 27) |

Ein Betreiber, der ein Hochrisikosystem einkauft, muss Anhang IV nicht erstellen. Er muss sie aber **erhalten** oder jedenfalls die Betriebsanleitung, weil Art. 26 die Verwendung nach Anleitung verlangt. Ein Anbieter, der keine liefert, erzeugt ein Problem auf der Betreiberseite.

## Der Weg zur Anbieterrolle, den niemand plant

Nach **Art. 25** wird ein Betreiber zum Anbieter, wenn er

1. seinen **Namen oder seine Marke** auf ein Hochrisikosystem setzt,
2. ein Hochrisikosystem **wesentlich ändert**,
3. die **Zweckbestimmung** so ändert, dass es zum Hochrisikosystem wird,
4. ein nicht als Hochrisiko bestimmtes System für einen **Hochrisikozweck** einsetzt.

Fall 1 bis 3 haben einen Anlass. **Fall 4 hat keinen:** kein Vertrag, keine Codeänderung. Es genügt, ein allgemeines Werkzeug in einem Anhang-III-Bereich einzusetzen.

### Was das für die Dokumentation bedeutet

Wer über Fall 4 zum Anbieter wird, hat die Anbieterpflichten **für ein System, das jemand anders gebaut hat**. Dann entsteht die unangenehme Lage:

| Anhang-IV-Abschnitt | Lage |
|---|---|
| allgemeine Beschreibung | aus Anbieterunterlagen machbar |
| Entwurfsentscheidungen | **liegen beim ursprünglichen Anbieter** |
| Datenherkunft, Training | **liegt beim ursprünglichen Anbieter** |
| Validierung und Test | für den eigenen Einsatzzweck selbst zu erbringen |
| Änderungsverlauf | ab dem eigenen Einsatz führbar |
| Risikomanagement | selbst zu erbringen |

Die zwei hervorgehobenen Zeilen sind der Grund, warum Fall 4 so teuer ist: Zwei Abschnitte kann man ohne Mitwirkung des Modellanbieters nicht füllen, und ein Anbieter, der ein allgemeines Werkzeug verkauft, hat keinen Grund, sie herauszugeben.

**Praktische Folge:** Die Frage, ob Fall 4 vorliegt, gehört vor den Einsatz, nicht danach. Sie lautet nicht „ist das Hochrisiko", sondern:

> Berührt die Ausgabe **Beschäftigung, Bildung, Kreditwürdigkeit, Strafverfolgung, Migration, Justiz, wesentliche Dienstleistungen oder kritische Infrastruktur**?

### Fall 2: wesentliche Änderung

Auch der zweite Fall betrifft dieses Repository unmittelbar. „Wesentlich" ist eine Änderung, die die Konformität oder die Zweckbestimmung berührt und die der Anbieter nicht vorab in seiner technischen Dokumentation bewertet hat.

**Wo die Frage gestellt werden muss:** im Freigabeschritt jeder Änderung, nicht im Jahresaudit. Deshalb hat die Änderungstabelle in der [Vorlage](../../templates/technical-documentation-template.md) eine eigene Spalte dafür. Sie zwingt dazu, die Frage laufend zu beantworten — und erzeugt dabei nebenbei den Nachweis, dass sie gestellt wurde.

## Weitere Rollen

| Rolle | Dokumentationsbezug |
|---|---|
| **Einführer** | muss prüfen, dass die technische Dokumentation vorliegt, und sie aufbewahren |
| **Händler** | muss prüfen, dass Kennzeichnung und Unterlagen vorhanden sind |
| **Bevollmächtigter** | hält die Dokumentation für einen Anbieter außerhalb der EU vor |

Wer ein KI-System aus einem Drittland in der EU weitergibt, ist möglicherweise Einführer — und dann ist das Fehlen der Dokumentation beim Hersteller das eigene Problem.

## Was in die Dokumentation über die Rolle gehört

| Feld | Inhalt |
|---|---|
| eigene Rolle | Anbieter / Betreiber, mit Begründung |
| Art. 25 geprüft | Datum, Ergebnis, auch bei Nein |
| bei Fall 4: berührter Anhang-III-Bereich | welcher |
| Fremdbestandteile | welches Modell, welche Version, welcher Anbieter |
| **welche Angaben der Anbieter nicht liefert** | mit Datum der Anfrage |

Die letzte Zeile ist die wichtigste in dieser Tabelle. Eine Lücke, die als Anbieterlücke dokumentiert ist, ist ein Befund gegen den Anbieter. Dieselbe Lücke ohne Dokumentation ist ein Befund gegen Sie.

## Weiter

[Wann Anhang IV greift](./risk-logic.md) · [Was laufend entstehen muss](./documentation-logic.md) · [AI Act für SaaS](https://github.com/SimpleAct-Compliance/simpleact-ai-act-for-saas)
