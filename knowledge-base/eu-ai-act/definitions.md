# Begriffe, an denen die Dokumentation hängt

Vier Begriffe entscheiden darüber, was in die Dokumentation gehört und wann sie ungültig wird.

## Zweckbestimmung (Art. 3 Nr. 12)

Die Verwendung, für die ein System vom Anbieter vorgesehen ist, einschließlich des Nutzungskontexts.

**In der Dokumentation:** Abschnitt 1 von Anhang IV, und die Grundlage für alles Weitere. Sie bestimmt, welche Risiken betrachtet werden müssen und was als Fehlanwendung gilt.

**Der Fehler, der Arbeit verursacht:** sie zu weit zu fassen. Eine breite Zweckbestimmung klingt nach Flexibilität und erweitert den Pflichtenkreis: Was man als vorgesehene Verwendung beschreibt, muss man auch bewerten, testen und dokumentieren.

**Praktisch bewährt:** die Zweckbestimmung eng fassen und in Abschnitt 3 ausdrücklich benennen, was das System **nicht** leistet und wofür es nicht eingesetzt werden darf.

## Vernünftigerweise vorhersehbare Fehlanwendung (Art. 3 Nr. 13)

Eine Verwendung, die nicht vorgesehen ist, sich aus menschlichem Verhalten oder dem Zusammenwirken mit anderen Systemen aber absehbar ergibt.

**In der Dokumentation:** Teil der Risikobetrachtung, und der Abschnitt, der am häufigsten leer bleibt, weil er nach Spekulation aussieht.

**Was hineingehört:** die Verwendung, die jemand schon versucht hat oder absehbar versuchen wird. Wird das Zusammenfassungswerkzeug für Personalentscheidungen benutzt werden? Nicht vorgesehen, aber absehbar — und in der Aufarbeitung eines Vorfalls wird ein leerer Abschnitt als unterlassene Betrachtung gelesen.

## Wesentliche Änderung (Art. 3 Nr. 23)

Eine Änderung nach dem Inverkehrbringen, die die Konformität oder die Zweckbestimmung berührt und die der Anbieter **nicht vorab in der technischen Dokumentation bewertet** hat.

**Der entscheidende Nebensatz** ist der letzte. Eine Änderung, die der Anbieter vorab bewertet und dokumentiert hat — etwa dass das Modell in einem beschriebenen Rahmen mit neuen Daten nachtrainiert und dabei überwacht wird — ist nicht wesentlich. Dieselbe Änderung ohne vorherige Bewertung ist es.

**Praktische Folge:** Wer absehbare Änderungen im Vorhinein in Anhang IV beschreibt, erspart sich später die Frage. Das ist einer der wenigen Fälle, in denen Dokumentationsarbeit unmittelbar Arbeit spart.

**Warum es die Rolle berührt:** Wer wesentlich ändert, kann nach Art. 25 zum Anbieter werden. Deshalb hat die Änderungstabelle eine eigene Spalte dafür.

## Version

Kein Begriff der Verordnung, und für die Dokumentation der wichtigste.

Jeder Nachweis bezieht sich auf einen Systemstand. Ohne Versionsangabe belegt er einen **Zeitpunkt**, nicht einen **Zustand** — und die Frage jeder Prüfung lautet: Welcher Stand war zu welchem Zeitpunkt in Betrieb?

**Was eine brauchbare Versionsangabe leistet:**

| Anforderung | Warum |
|---|---|
| eindeutig | zwei Nachweise müssen demselben Stand zuordenbar sein |
| im System ablesbar | sonst ist sie nicht überprüfbar |
| in der Änderungstabelle geführt | sonst ist die Reihenfolge unklar |
| umfasst Fremdbestandteile | ein Modellwechsel beim Zulieferer ist eine Änderung |

Die letzte Zeile wird übersehen. Wenn die eigene Version gleich bleibt, der Anbieter eines eingebetteten Modells aber getauscht hat, ist das System ein anderes — und alle Nachweise zu Genauigkeit und Verhalten beziehen sich auf etwas, das es nicht mehr gibt.

## Was dieses Repository nicht definiert

Konformitätsbewertung, benannte Stelle, CE-Kennzeichnung, Registrierung in der EU-Datenbank. Diese Begriffe gehören zum Verfahren **nach** der Dokumentation. Wer bei Anhang IV steht, hat sie noch vor sich — und braucht dafür in der Regel rechtliche oder zertifizierungsseitige Begleitung.

## Weiter

[Wer dokumentieren muss](./scope-and-actors.md) · [Was laufend entstehen muss](./documentation-logic.md) · [Die Nachweisschicht](./evidence-layer.md)
