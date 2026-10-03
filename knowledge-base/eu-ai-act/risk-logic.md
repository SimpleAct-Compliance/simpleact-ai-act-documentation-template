# Wann Anhang IV greift

Die Dokumentationspflicht nach Art. 11 hängt an zwei Bedingungen: **Hochrisiko** und **Anbieterrolle**. Fehlt eine, besteht sie nicht — was nicht bedeutet, dass nichts zu dokumentieren wäre.

## Die Prüfung in zwei Schritten

```
  1 Ist es ein Hochrisikosystem?   Anhang I oder Anhang III
  2 Sind wir Anbieter?             Art. 3 Nr. 3 oder Art. 25
```

Beide Ja: Anhang IV gilt. Ein Nein: Anhang IV gilt nicht, und es bleiben die Pflichten aus der nächsten Tabelle.

## Was bei anderen Klassen zu dokumentieren ist

| Klasse | Dokumentation |
|---|---|
| **Verboten** (Art. 5) | die Entscheidung, den Betrieb einzustellen, mit Datum und Begründung — und was stattdessen geschieht |
| **Hochrisiko, Betreiberrolle** | Protokolle (Art. 26), Verwendung nach Anleitung, ggf. Grundrechte-Folgenabschätzung (Art. 27) |
| **Transparenzpflicht** (Art. 50) | Kennzeichnung, Nachweis mit **Datum und Produktversion** |
| **Minimal** | Inventareintrag, Einstufungsbegründung, Schulungsstand (Art. 4) |

Die erste Zeile wird vergessen. Ein Werkzeug abzuschalten ist die richtige Reaktion auf einen Art.-5-Treffer — und ohne Dokumentation ist später nicht erkennbar, dass die Prüfung stattgefunden hat und zu einer Entscheidung geführt hat.

## Anhang I gegen Anhang III

| | Anhang I | Anhang III |
|---|---|---|
| Anknüpfung | Sicherheitsbauteil eines Produkts mit bestehender Konformitätsbewertung | acht Einsatzbereiche |
| Beispiele | Maschinen, Medizinprodukte, Fahrzeuge, Aufzüge | Beschäftigung, Kreditwürdigkeit, Bildung, Biometrie |
| Anwendbar ab | 2.8.2028 | **2.12.2027** |
| Verfahren | läuft im bestehenden Konformitätsverfahren mit | eigenständig |

**Für die Dokumentation wichtig:** Bei Anhang I existiert meist schon eine technische Dokumentation nach der jeweiligen Produktvorschrift. Anhang IV wird dann nicht daneben geschrieben, sondern eingearbeitet. Wer zwei getrennte Dokumentationen führt, hat nach einem Jahr Widersprüche zwischen ihnen.

## Die Ausnahme nach Art. 6 Abs. 3

Ein System in einem Anhang-III-Bereich ist nicht hochriskant, wenn es nur eine eng begrenzte Verfahrensaufgabe erfüllt, ein menschliches Ergebnis verbessert, Muster erkennt ohne die Bewertung zu ersetzen, oder vorbereitend tätig ist.

Zwei Punkte, die für dieses Repository zählen:

**Die Bewertung ist selbst ein Dokument.** Die Verordnung verlangt, dass die Einschätzung dokumentiert wird. Wer sich auf die Ausnahme beruft, hat also nicht weniger zu dokumentieren, sondern anderes: statt Anhang IV eine nachvollziehbare Begründung, warum die Ausnahme trägt.

**Die Rückausnahme:** Wird **Profiling** natürlicher Personen vorgenommen, greift die Ausnahme nicht — unabhängig von allen vier Tatbeständen. Sie steht nach der Aufzählung und wird beim Lesen oft übersprungen.

## Was die Einstufung für die Dokumentation liefern muss

| Angabe | Wofür in Anhang IV |
|---|---|
| Einsatzzweck, abgegrenzt | Abschnitt 1, Zweckbestimmung |
| berührter Anhang-III-Bereich | ob die Pflicht überhaupt greift |
| Rolle und Art.-25-Prüfung | wer dokumentiert |
| Betroffenenkreis | Abschnitt 2, Annahmen über betroffene Personen |
| Grad der menschlichen Aufsicht | Abschnitt 2, Aufsicht |
| Datenarten und Herkunft | Abschnitt 2, Datenanforderungen |
| Annahmen der Einstufung | Abschnitt 3, Grenzen |

Die letzte Zeile ist eine nützliche Verbindung: Was bei der Einstufung als **Annahme** festgehalten wurde, gehört in Anhang IV als **Grenze** des Systems. Beides beschreibt dasselbe — was man nicht weiß oder nicht garantieren kann.

## Ein System, mehrere Einsatzzwecke

Eingestuft wird ein Einsatzzweck, nicht ein Werkzeug. Für die Dokumentation heißt das nicht zwangsläufig: mehrere Dokumentationen.

| Lage | Dokumentation |
|---|---|
| ein System, ein Einsatzzweck, hochriskant | eine Anhang-IV-Dokumentation |
| ein System, mehrere Zwecke, einer hochriskant | eine Dokumentation, die die Zweckbestimmung eng fasst, plus Begründung für die anderen Zwecke |
| mehrere Systeme, je hochriskant | je System eine |

Der mittlere Fall ist der häufige und der kniffligste. Praktisch bewährt: die Zweckbestimmung in Abschnitt 1 **eng** beschreiben und in Abschnitt 3 ausdrücklich benennen, was das System nicht leistet und wofür es nicht eingesetzt werden darf. Das ist gleichzeitig der Teil, auf den sich Betreiber verlassen.

## Weiter

[Was laufend entstehen muss](./documentation-logic.md) · [Die Nachweisschicht](./evidence-layer.md) · [Risikoeinstufung](https://github.com/SimpleAct-Compliance/simpleact-ai-risk-classification-eu)
