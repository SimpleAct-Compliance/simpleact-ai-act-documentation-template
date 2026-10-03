# Was laufend entstehen muss

Anhang IV hat neun Abschnitte. Vier davon entstehen während der Entwicklung oder gar nicht. Die übrigen sind Schreibarbeit und jederzeit nachholbar.

Diese Unterscheidung ist der praktisch wichtigste Inhalt dieses Repositories, weil sie bestimmt, **was man heute tun muss**, auch wenn die Frist 2027 ist.

---

## Die vier, die nicht nachholbar sind

### 1 Entwurfsentscheidungen mit Begründung

**Was Anhang IV verlangt:** die Entwurfsspezifikationen, die Architektur, und die Entscheidungen samt Begründung — einschließlich der Annahmen über die Personen, auf die das System angewandt wird.

**Warum nicht nachholbar:** Nach zwei Jahren weiß niemand mehr, welche Alternative verworfen wurde und aus welchem Grund. Was dann entsteht, ist eine Rekonstruktion: plausibel, unbelegt, und in einer Prüfung als solche erkennbar.

**Was während der Entwicklung genügt:** ein kurzer Eintrag je Entscheidung — was wurde entschieden, welche Alternativen standen zur Wahl, warum diese. Vier Sätze, nicht vier Seiten.

**Wo er hingehört:** dorthin, wo die Entscheidung fällt. Ein Architekturentscheidungsprotokoll im Repository ist dafür besser geeignet als ein Dokument, das jemand später zusammenträgt.

### 2 Datenherkunft und Aufbereitung

**Was Anhang IV verlangt:** Herkunft der Daten, Umfang, Hauptmerkmale, Art der Beschaffung, Kennzeichnung, Bereinigung — und bei personenbezogenen Daten die Rechtsgrundlage.

**Warum nicht nachholbar:** Welche Quelle wann mit welchem Schritt bereinigt wurde, steht in keinem Repository. Es steht in den Köpfen der Leute, die es gemacht haben, und verschwindet mit ihnen.

**Was genügt:** eine Tabelle je Datenquelle, laufend geführt: Quelle, Zeitraum, Umfang, Rechtsgrundlage, Bereinigungsschritte, bekannte Verzerrungen.

Die letzte Spalte ist die unangenehme und die wertvollste. Eine bekannte Verzerrung, die dokumentiert ist, ist ein Nachweis von Sorgfalt; dieselbe Verzerrung, die später auffällt, ist ein Befund.

### 3 Validierung und Testergebnisse

**Was Anhang IV verlangt:** die angewandten Validierungs- und Testverfahren, die Metriken, die Ergebnisse — und die Testprotokolle, datiert und unterzeichnet.

**Warum nicht nachholbar:** Tests lassen sich wiederholen. Die Ergebnisse der damaligen Version nicht. Wenn in einer Prüfung die Genauigkeit zum Zeitpunkt eines Vorfalls gefragt wird, hilft ein heutiger Testlauf nicht.

**Was genügt:** je Version ein Testprotokoll mit Datum, Metrik, Ergebnis und Testdatensatz-Kennung. Die **Reihe** ist der Nachweis, nicht der letzte Lauf.

### 4 Änderungsverlauf

**Was Anhang IV verlangt:** die Liste der Änderungen, die am System über seinen Lebenszyklus vorgenommen wurden.

**Warum nicht nachholbar:** Ein Änderungsverlauf, der nachträglich aus Commit-Nachrichten und Erinnerungen zusammengesetzt wird, hat genau dort Lücken, wo etwas Unangenehmes passiert ist.

**Warum es der wichtigste Abschnitt ist:** Er beantwortet die Frage, die jede Prüfung stellt — **welcher Stand war zu welchem Zeitpunkt in Betrieb?** Ohne ihn lässt sich kein anderer Nachweis zeitlich zuordnen.

**Was genügt:**

| Datum | Änderung | Wesentlich nach Art. 3 Nr. 23? | Folge | Durch |
|---|---|---|---|---|
| | | | | |

Die dritte Spalte ist der Punkt, an dem die Rollenfrage wieder auftaucht: Wer wesentlich ändert, kann zum Anbieter werden. Die Spalte zwingt dazu, die Frage bei jeder Änderung zu stellen, statt einmal im Jahr.

---

## Die fünf, die Schreibarbeit sind

| Abschnitt | Aufwand | Nachholbar |
|---|---|---|
| allgemeine Beschreibung, Zweckbestimmung, Version | gering | ja |
| Betriebsanleitung für Betreiber | mittel | ja |
| Angaben zu Genauigkeit, Robustheit, Cybersicherheit | gering, **wenn** Messwerte existieren | teilweise |
| angewandte harmonisierte Normen | gering | ja |
| EU-Konformitätserklärung | gering | ja |

Die dritte Zeile ist der Grenzfall: Die Beschreibung ist Schreibarbeit, die **Messwerte** sind es nicht. Wer nie gemessen hat, kann nicht nachträglich sagen, wie genau das System vor einem Jahr war.

## Was daraus für heute folgt

Auch wenn Anhang III erst ab 2.12.2027 anwendbar ist, sind drei Dinge jetzt zu tun — vorausgesetzt, man könnte Anbieter sein:

1. **Entwurfsentscheidungen festhalten**, ab sofort, in vier Sätzen je Entscheidung
2. **Änderungsverlauf beginnen**, mit der Spalte zur Wesentlichkeit
3. **Testläufe datieren und ablegen**, auch wenn die Metriken noch nicht endgültig sind

Alle drei kosten wenig und sind nicht einholbar. Das ist der Grund, warum die Verschiebung weniger Zeit verschafft, als sie aussieht.

## Die Betriebsanleitung ist kein Nebenprodukt

Art. 13 verlangt, dass Betreiber die Ausgaben auslegen können. Die Betriebsanleitung ist damit nicht Dokumentation **über** das System, sondern Teil des Produkts — und der Teil, auf den sich Betreiber verlassen, wenn sie ihre eigenen Pflichten nach Art. 26 erfüllen.

Was darin oft fehlt und fehlen darf, aber nicht sollte:

- die **Grenzen**: was das System nicht leistet
- die vorhersehbaren **Fehlerarten**, mit Beispielen
- was ein Betreiber **nicht** damit tun darf
- woran eine falsche Ausgabe erkennbar ist

Der letzte Punkt entscheidet darüber, ob die menschliche Aufsicht beim Betreiber überhaupt funktionieren kann.

## Weiter

[Die Nachweisschicht](./evidence-layer.md) · [Vorlage](../../templates/technical-documentation-template.md) · [Woher die Angaben kommen](./inventory-and-governance.md)
