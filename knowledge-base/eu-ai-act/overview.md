# Was wann gilt

## Die Fristen für die Dokumentationspflicht

Nach dem **Digital Omnibus** (Verordnung (EU) 2026/1744, in Kraft seit 27.7.2026):

| Hochrisiko nach | Anwendbar ab | Verschoben |
|---|---|---|
| **Anhang III** | **2.12.2027** | ja, um 16 Monate |
| Anhang I | 2.8.2028 | nein |
| Bestandssysteme bei Behörden | 2.8.2030 | nein |

Die technische Dokumentation nach Art. 11 und Anhang IV hängt an der Hochrisiko-Einstufung. Ohne Hochrisikosystem besteht diese Pflicht nicht.

## Warum die Verschiebung weniger Zeit verschafft, als sie aussieht

Vier Abschnitte von Anhang IV entstehen während der Entwicklung oder gar nicht: Entwurfsentscheidungen, Datenherkunft, Testergebnisse, Änderungsverlauf.

Wer bis Mitte 2027 wartet und dann anfängt, hat für diese vier nichts in der Hand. Was dann entsteht, ist eine Rekonstruktion — plausibel, unbelegt, und in einer Prüfung als solche erkennbar.

**Was daraus folgt:** Drei Dinge sind jetzt zu tun, auch ohne Frist, vorausgesetzt man könnte Anbieter sein:

1. Entwurfsentscheidungen festhalten, vier Sätze je Entscheidung
2. Änderungsverlauf beginnen, mit der Spalte zur Wesentlichkeit
3. Testläufe datieren und ablegen

Alle drei kosten wenig und sind nicht einholbar. Ausführlich: [Was laufend entstehen muss](./documentation-logic.md)

## Was heute gilt, unabhängig von Anhang IV

Drei Pflichten sind anwendbar und erzeugen eigene Dokumentation — auch für Betreiber, auch ohne Hochrisikosystem:

| Pflicht | Seit | Was zu dokumentieren ist |
|---|---|---|
| **Art. 5** verbotene Praktiken | 2.2.2025 | Prüfergebnis je Praktik, mit Datum |
| **Art. 4** KI-Kompetenz | 2.2.2025 | wer geschult wurde, wann, zu welchem Inhalt |
| **Art. 50** Transparenz | 2.8.2026 | Kennzeichnung mit **Datum und Produktversion** |

Diese drei sind der Teil mit Frist in der Vergangenheit. Sie sind klein, und sie werden regelmäßig übersehen, weil die Aufmerksamkeit bei Anhang IV liegt.

## Und die Dokumentation nach DSGVO

Sie läuft parallel und greift auf dieselben Angaben zu:

| DSGVO | Berührung zu Anhang IV |
|---|---|
| Art. 30 Verarbeitungsverzeichnis | Datenarten, Zweck, Empfänger, Verarbeitungsort |
| Art. 6 und 9 Rechtsgrundlage | gehört ohnehin in die Datenquellentabelle |
| Art. 28 Auftragsverarbeitung | Fremdbestandteile, Unterauftragsverarbeiter |
| Art. 35 DSFA | Risikobewertung, teilweise deckungsgleich |

Wer beides getrennt erhebt, macht die Arbeit zweimal — und hat nach einem halben Jahr an einer von beiden Stellen veraltete Angaben.

Bei Hochrisiko kommt außerdem die **Grundrechte-Folgenabschätzung nach Art. 27 AI Act** in Betracht. Sie ist nicht die DSFA und ersetzt sie nicht, kann aber auf denselben Erhebungen aufbauen.

## Der Aufbau von Anhang IV

Neun Abschnitte:

```
  1 allgemeine Beschreibung, Zweckbestimmung, Version
  2 Entwicklung, Architektur, Daten, Aufsicht, Validierung
  3 Überwachung, Funktionsweise, Kontrolle, Grenzen
  4 Risikomanagementsystem (Art. 9)
  5 Änderungen am Lebenszyklus
  6 angewandte harmonisierte Normen
  7 EU-Konformitätserklärung
  8 Beobachtung nach dem Inverkehrbringen (Art. 72)
```

Abschnitt 2 ist der aufwendigste. Abschnitt 5 ist der praktisch wichtigste, weil er die Frage beantwortet, die jede Prüfung stellt: welcher Stand war zu welchem Zeitpunkt in Betrieb?

## Weiter

[Wer dokumentieren muss](./scope-and-actors.md) · [Was laufend entstehen muss](./documentation-logic.md) · [Vorlage](../../templates/technical-documentation-template.md)
