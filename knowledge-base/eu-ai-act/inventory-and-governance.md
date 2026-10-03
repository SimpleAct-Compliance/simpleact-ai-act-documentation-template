# Woher die Angaben kommen

Anhang IV ist keine Schreibaufgabe, sondern eine Sammelaufgabe. Der größte Teil der Angaben liegt bereits irgendwo — verstreut, und bei Leuten, die nicht wissen, dass sie gebraucht werden.

## Wer was liefert

| Abschnitt | Wer liefert |
|---|---|
| Zweckbestimmung, Nutzergruppen | Produkt oder Fachbereich |
| Architektur, Entwurfsentscheidungen | Entwicklung |
| Datenherkunft, Aufbereitung, Rechtsgrundlage | Entwicklung und Datenschutz |
| Validierung, Testergebnisse | Entwicklung oder Qualitätssicherung |
| Genauigkeit, Robustheit, Cybersicherheit | Entwicklung und IT-Sicherheit |
| menschliche Aufsicht | Fachbereich, der sie ausübt |
| Grenzen und Fehlerarten | Entwicklung **und** Fachbereich |
| Risikomanagement | Compliance, mit Zuarbeit |
| Änderungsverlauf | Entwicklung, laufend |
| Fremdbestandteile und Anbieterzusagen | Beschaffung |

Zwei Zeilen sind besonders. **Menschliche Aufsicht** kann nur der Fachbereich beantworten, der sie tatsächlich ausübt — und zwar mit der unbequemen Zahl, wie viele Ausgaben im letzten Monat geändert wurden. Und **Grenzen und Fehlerarten** braucht beide Seiten: Die Entwicklung weiß, was das Modell nicht kann; der Fachbereich weiß, wo das im Alltag zu falschen Ergebnissen führt.

## Was das Inventar liefern muss

Ohne Inventareintrag beginnt die Dokumentation mit einer Suche nach Grundangaben.

| Inventarangabe | Anhang-IV-Abschnitt |
|---|---|
| Einsatzzweck, abgegrenzt | 1 |
| Anbieter, Modell, **Version** | 1 und 5 |
| Datenarten, Verarbeitungsort | 2 |
| Betroffenenkreis | 2 |
| Grad der Aufsicht | 2 und 3 |
| berührter Anhang-III-Bereich | ob die Pflicht greift |

Dazu: [KI-Inventar](https://github.com/SimpleAct-Compliance/simpleact-ai-system-inventory)

## Die Angaben, die vom Anbieter kommen müssen

Bei Fremdbestandteilen — einem zugekauften Modell, einer eingebetteten Komponente — gibt es Abschnitte, die ohne Mitwirkung des Anbieters nicht füllbar sind:

- Trainingsdatenherkunft
- Entwurfsentscheidungen des Modells
- Genauigkeitsangaben der Grundkomponente
- Modellversion und Änderungsverlauf

**Was zu tun ist, wenn der Anbieter nicht liefert:** die Lücke benennen, mit Datum der Anfrage und der Antwort, die er gegeben hat. Dann ist es ein Befund gegen den Anbieter und gehört in die Beschaffung. Ohne Dokumentation ist es ein Befund gegen Sie.

Dazu: [Anbieterregister](https://github.com/SimpleAct-Compliance/simpleact-model-vendor-register)

## Zuständigkeit

| Rolle | Aufgabe |
|---|---|
| **Dokumentationsverantwortlicher** | hält die Gliederung, sammelt, erinnert; schreibt nicht alles selbst |
| **Zuliefernde** je Abschnitt | liefern Inhalt, mit Namen am Abschnitt |
| **Prüfer** | sieht nach, ob die Abschnitte stimmen — nicht ob sie gefüllt sind |
| **Freigebender** | bestätigt je Version |

Der häufigste Fehler ist, die Dokumentation einer Person zu geben, die sie **schreiben** soll. Dann entstehen die Abschnitte, die diese Person beurteilen kann, und der Rest wird mit Worten gefüllt.

Besser: Die Gliederung steht, je Abschnitt ist ein Name eingetragen, und die Verantwortliche sammelt und erinnert. Das verteilt die Arbeit dorthin, wo das Wissen sitzt.

## Wo die Dokumentation leben sollte

| Ort | Taugt für | Problem |
|---|---|---|
| Textdokument auf einem Laufwerk | nichts davon | keine Versionierung, keine Zuständigkeit je Abschnitt |
| Wiki | Abschnitte 1, 3, 6, 7 | Änderungsverlauf unzuverlässig |
| Repository, in Markdown | alles, besonders 2 und 5 | braucht Zugang für Nicht-Entwickler |
| Fachanwendung | alles, mit Freigabeläufen | Einführungsaufwand |

Entscheidend ist nicht der Ort, sondern dass **Abschnitt 5** — der Änderungsverlauf — dort liegt, wo Änderungen tatsächlich stattfinden. Ein Änderungsverlauf, der an einer anderen Stelle gepflegt werden muss als die Änderung selbst, wird nicht gepflegt.

## Wann die Dokumentation beginnt

Nicht wenn die Frist näher kommt. Die vier nicht nachholbaren Abschnitte — Entwurfsentscheidungen, Datenherkunft, Testergebnisse, Änderungsverlauf — beginnen mit der Entwicklung oder gar nicht.

Für ein System, das heute schon läuft, ist der ehrliche Weg: ab jetzt lückenlos führen, und den Zeitraum davor als **benannte Lücke** stehen lassen. Das ist weniger wert als eine vollständige Dokumentation und wesentlich mehr als eine Rekonstruktion, die in der Prüfung auffällt.

## Weiter

[Was laufend entstehen muss](./documentation-logic.md) · [Dokumentationsprüfung](../../templates/documentation-checklist.md)
