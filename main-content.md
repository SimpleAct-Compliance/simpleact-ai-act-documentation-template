# Technische Dokumentation nach Anhang IV — Volltext

Dieses Dokument fasst das Repository in einem Stück zusammen.

## Der Ausgangspunkt

Das meiste von Anhang IV lässt sich nicht nachträglich schreiben. Entwurfsentscheidungen, Datenherkunft, Testergebnisse und Änderungsverlauf entstehen während der Entwicklung oder gar nicht. Was später entsteht, ist eine Rekonstruktion: plausibel, unbelegt, und in einer Prüfung als solche erkennbar.

Diese Unterscheidung bestimmt, was heute zu tun ist — auch wenn Anhang III erst ab **2.12.2027** anwendbar ist (Digital Omnibus, Verordnung (EU) 2026/1744, um 16 Monate verschoben) und Anhang I ab 2.8.2028.

## Wen die Pflicht trifft

Die technische Dokumentation nach Art. 11 und Anhang IV ist eine **Anbieterpflicht** für Hochrisikosysteme. Betreiber brauchen sie nicht — sie müssen aber die Betriebsanleitung haben, weil Art. 26 die Verwendung nach Anleitung verlangt.

Der Haken liegt in **Art. 25**: Ein Betreiber wird zum Anbieter, wenn er seinen Namen auf ein Hochrisikosystem setzt, es wesentlich ändert, seine Zweckbestimmung ändert — oder ein nicht als Hochrisiko bestimmtes System für einen Hochrisikozweck einsetzt. Die ersten drei Fälle haben einen Anlass; der vierte hat keinen.

Wer über den vierten Fall zum Anbieter wird, hat die Anbieterpflichten für ein System, das jemand anders gebaut hat. Dann sind zwei Abschnitte ohne Mitwirkung des ursprünglichen Anbieters nicht füllbar: Entwurfsentscheidungen und Trainingsdatenherkunft. Ein Anbieter, der ein allgemeines Werkzeug verkauft, hat keinen Grund, sie herauszugeben. Deshalb gehört die Frage vor den Einsatz: Berührt die Ausgabe Beschäftigung, Bildung, Kreditwürdigkeit, Strafverfolgung, Migration, Justiz, wesentliche Dienstleistungen oder kritische Infrastruktur?

## Die vier nicht nachholbaren Abschnitte

**Entwurfsentscheidungen mit Begründung.** Nach zwei Jahren weiß niemand mehr, welche Alternative verworfen wurde und warum. Während der Entwicklung genügen vier Sätze je Entscheidung — was wurde entschieden, welche Alternativen standen zur Wahl, warum diese. Der Ort dafür ist dort, wo die Entscheidung fällt, nicht in einem Dokument, das jemand später zusammenträgt.

**Datenherkunft und Aufbereitung.** Welche Quelle wann mit welchem Schritt bereinigt wurde, steht in keinem Repository, sondern in den Köpfen der Leute, die es gemacht haben. Eine Tabelle je Datenquelle genügt: Quelle, Zeitraum, Umfang, Rechtsgrundlage, Bereinigungsschritte, bekannte Verzerrungen. Die letzte Spalte ist die unangenehme und die wertvollste — eine dokumentierte Verzerrung ist ein Nachweis von Sorgfalt, dieselbe Verzerrung später ist ein Befund.

**Validierung und Testergebnisse.** Tests lassen sich wiederholen, die Ergebnisse der damaligen Version nicht. Wird in einer Prüfung die Genauigkeit zum Zeitpunkt eines Vorfalls gefragt, hilft ein heutiger Testlauf nicht. Die Reihe der Protokolle ist der Nachweis, nicht der letzte Lauf.

**Änderungsverlauf.** Nachträglich aus Commit-Nachrichten und Erinnerungen zusammengesetzt, hat er Lücken genau dort, wo etwas Unangenehmes passiert ist. Er ist der praktisch wichtigste Abschnitt, weil er die Frage beantwortet, die jede Prüfung stellt: **Welcher Stand war zu welchem Zeitpunkt in Betrieb?** Ohne ihn lässt sich kein anderer Nachweis zeitlich zuordnen.

Die Änderungstabelle braucht eine Spalte zur **Wesentlichkeit nach Art. 3 Nr. 23**. Sie zwingt dazu, die Rollenfrage bei jeder Änderung zu stellen statt einmal im Jahr — und erzeugt dabei den Nachweis, dass sie gestellt wurde. Und sie muss **Modellwechsel bei Fremdbestandteilen** aufnehmen: Bleibt die eigene Version gleich, hat der Zulieferer aber getauscht, ist das System ein anderes, und alle Nachweise zu Genauigkeit und Verhalten beziehen sich auf etwas, das es nicht mehr gibt.

## Die fünf, die Schreibarbeit sind

Allgemeine Beschreibung, Betriebsanleitung, Angaben zu Genauigkeit und Robustheit, Normen, Konformitätserklärung. Jederzeit nachholbar — mit einem Grenzfall: Die Beschreibung der Genauigkeit ist Schreibarbeit, die **Messwerte** sind es nicht.

Die Betriebsanleitung ist dabei kein Nebenprodukt. Art. 13 verlangt, dass Betreiber die Ausgaben auslegen können; sie ist damit Teil des Produkts und der Teil, auf den sich Betreiber verlassen, wenn sie ihre eigenen Pflichten erfüllen. Was darin oft fehlt: die Grenzen, die vorhersehbaren Fehlerarten mit Beispielen, was ein Betreiber nicht damit tun darf, und woran eine falsche Ausgabe erkennbar ist. Der letzte Punkt entscheidet darüber, ob die menschliche Aufsicht beim Betreiber überhaupt funktionieren kann.

## Dokumentation ist nicht Nachweis

Die Dokumentation ist eine Beschreibung, die auf Nachweise verweist. „Das System erreicht 94 % Genauigkeit auf dem Validierungsdatensatz" ist Dokumentation; das Testprotokoll mit Datum, Datensatz-Kennung, Metrik und Ergebnis ist der Nachweis. Ohne Protokoll ist der Satz eine Zahl, die jemand aufgeschrieben hat.

Jeder Nachweis trägt fünf Bestandteile: **Version**, Datum, Fundort, Urheber, Bezug zum Abschnitt. Die letzte wird unterschätzt — ein Ordner mit vierzig Dateien, von denen niemand sagen kann, welchen Abschnitt welche belegt, ist in einer Prüfung ein Ordner mit vierzig Dateien.

Der am schwersten zu beschaffende und aussagekräftigste Nachweis ist der zur **menschlichen Aufsicht**: Die Dokumentation kann beschreiben, dass Aufsicht technisch ermöglicht wird; dass sie ausgeübt wird, belegt nur eine Zahl — wie viele Ausgaben im Betrieb geändert oder verworfen wurden.

## Woher die Angaben kommen

Anhang IV ist eine Sammelaufgabe. Der häufigste Fehler ist, die Dokumentation einer Person zu geben, die sie schreiben soll: Dann entstehen die Abschnitte, die diese Person beurteilen kann, und der Rest wird mit Worten gefüllt.

Besser: Die Gliederung steht, je Abschnitt ist ein Name eingetragen, und eine Verantwortliche sammelt und erinnert. Zwei Abschnitte brauchen zwingend den Fachbereich — die Betriebszahl zur Aufsicht, und die Grenzen und Fehlerarten, für die beide Seiten gebraucht werden: Die Entwicklung weiß, was das Modell nicht kann, der Fachbereich weiß, wo das im Alltag zu falschen Ergebnissen führt.

Bei Fremdbestandteilen gibt es Abschnitte, die ohne den Anbieter nicht füllbar sind. Was dann zu tun ist: die Lücke benennen, mit Datum der Anfrage und der Antwort. Dann ist es ein Befund gegen den Anbieter und gehört in die Beschaffung — ohne Dokumentation ist es ein Befund gegen Sie.

## Lücken benennen, nicht füllen

Ein Abschnitt mit „liegt nicht vor, verantwortlich ___, Termin ___" ist besser als einer mit Füllsätzen. Füllsätze fallen auf und stellen den Rest in Frage: Wer einen Abschnitt erkennbar mit Worten gefüllt hat, hat möglicherweise mehrere so gefüllt. Eine benannte Lücke zeigt dagegen, dass jemand den Abschnitt gelesen und verstanden hat.

Für ein System, das heute schon läuft, ist der ehrliche Weg: ab jetzt lückenlos führen, und den Zeitraum davor als benannte Lücke stehen lassen.

## Weg durch das Repository

1. [Wer dokumentieren muss](./knowledge-base/eu-ai-act/scope-and-actors.md) — erst die Rollenfrage
2. [Wann Anhang IV greift](./knowledge-base/eu-ai-act/risk-logic.md)
3. [Was laufend entstehen muss](./knowledge-base/eu-ai-act/documentation-logic.md) — der praktische Kern
4. [Die Nachweisschicht](./knowledge-base/eu-ai-act/evidence-layer.md)
5. [Woher die Angaben kommen](./knowledge-base/eu-ai-act/inventory-and-governance.md)
6. [Vorlage](./templates/technical-documentation-template.md) — Gliederung anlegen, je Abschnitt einen Namen
7. [Dokumentationsprüfung](./templates/documentation-checklist.md) — durch eine andere Person

---

Keine Rechtsberatung. Stand: Oktober 2026.
