# Vorlagen

Zwei Dokumente: eines zum Führen, eines zum Nachsehen.

| Vorlage | Zweck | Wer |
|---|---|---|
| [Technische Dokumentation](./technical-documentation-template.md) | Anhang IV, Abschnitt für Abschnitt, mit Hinweis je Abschnitt | Dokumentationsverantwortlicher, mit Zuarbeit |
| [Dokumentationsprüfung](./documentation-checklist.md) | ist das vorzeigbar? | eine andere Person |

Die zweite ist nicht optional. Wer seine eigene Dokumentation prüft, sieht, was er geschrieben hat, und nicht, was fehlt.

## Was an der Vorlage anders ist

**Je Abschnitt steht, wer liefert.** Der häufigste Fehler ist, die Dokumentation einer Person zu geben, die sie schreiben soll. Dann entstehen die Abschnitte, die diese Person beurteilen kann, und der Rest wird mit Worten gefüllt. Die Vorlage verteilt die Arbeit dorthin, wo das Wissen sitzt.

**Vier Abschnitte sind als nicht nachholbar gekennzeichnet.** Entwurfsentscheidungen, Datenherkunft, Testprotokolle, Änderungsverlauf. Diese Markierung ist der praktische Kern: Sie sagt, was heute zu tun ist, auch wenn die Frist 2027 ist.

**Die Änderungstabelle hat eine Spalte zur Wesentlichkeit.** Damit wird die Rollenfrage nach Art. 25 bei jeder Änderung gestellt statt einmal im Jahr — und der Nachweis, dass sie gestellt wurde, entsteht nebenbei.

**Zur menschlichen Aufsicht wird eine Betriebszahl verlangt.** Wie viele Ausgaben wurden im letzten Monat geändert oder verworfen? Alles andere belegt nur, dass Aufsicht möglich ist.

## Reihenfolge beim ersten Mal

1. **Rolle klären.** Ohne Anbieterrolle gilt Anhang IV nicht. Siehe [Wer dokumentieren muss](../knowledge-base/eu-ai-act/scope-and-actors.md).
2. **Gliederung anlegen** und je Abschnitt einen **Namen** eintragen — vor dem Schreiben.
3. **Die vier nicht nachholbaren Abschnitte beginnen**, ab sofort, auch unvollständig.
4. Die übrigen Abschnitte füllen, in beliebiger Reihenfolge.
5. **Dokumentationsprüfung** durch eine andere Person.

Schritt 3 vor Schritt 4: Die Schreibarbeit ist jederzeit nachholbar, die laufenden Abschnitte nicht.

## Lücken benennen, nicht füllen

Ein Abschnitt mit „liegt nicht vor, verantwortlich ___, Termin ___, weil der Anbieter die Angabe nicht herausgibt, angefragt am ___" ist in einer Prüfung besser als ein Abschnitt mit Füllsätzen.

Füllsätze fallen auf und stellen den Rest in Frage. Eine benannte Lücke zeigt dagegen, dass jemand den Abschnitt gelesen und verstanden hat.

## Format

Markdown, damit die Dokumentation versionierbar ist und ein Diff zeigt, was sich zwischen zwei Fassungen geändert hat.

Für Anhang IV ist das nicht Komfort, sondern inhaltlich: Abschnitt 5 verlangt den Änderungsverlauf, und ein Änderungsverlauf, der an einer anderen Stelle gepflegt werden muss als die Änderung selbst, wird nicht gepflegt. Eine Dokumentation im Repository, neben dem Code, löst dieses Problem von selbst.

## Weiter

[Was laufend entstehen muss](../knowledge-base/eu-ai-act/documentation-logic.md) · [Die Nachweisschicht](../knowledge-base/eu-ai-act/evidence-layer.md) · [README](../README.md)
