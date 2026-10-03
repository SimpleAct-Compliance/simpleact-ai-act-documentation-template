# Mitwirken

Dieses Repository beschreibt eine Dokumentationspflicht, kein Produkt. Es lebt davon, dass Leute aus der Praxis widersprechen.

## Besonders willkommen

- **Abschnitte, die in einer Prüfung oder Konformitätsbewertung tatsächlich gelesen wurden** — und welche niemand sehen wollte
- **Erfahrungen mit nachträglicher Dokumentation**: welcher Abschnitt sich wie weit rekonstruieren ließ, und wo es auffiel
- **Anbieterlücken**: welche Angaben Modellanbieter in der Praxis liefern und welche nicht
- **Formulierungen für den Abschnitt Grenzen**, die etwas taugen. Das ist der am schwersten zu schreibende Teil
- **Korrekturen an Rechtsbezügen** — mit Fundstelle; Anhang- und Abschnittsnummern sind hier das Wichtigste
- **Übersetzungen** einzelner Dokumente

Am wertvollsten sind Rückmeldungen zur Trennung zwischen nachholbaren und nicht nachholbaren Abschnitten. Sie ist die inhaltliche Hauptaussage dieses Repositories, und wenn sie in einem Fall nicht trägt, gehört das hierher.

## Weniger hilfreich

- **Vollständigere Gliederungen.** Anhang IV hat neun Abschnitte; mehr Unterpunkte machen die Vorlage nicht brauchbarer
- **Beispieltexte für Abschnitte.** Ein ausformulierter Beispielabschnitt wird abgeschrieben, und abgeschriebene Abschnitte fallen in einer Prüfung als Füllsätze auf. Die Vorlage sagt deshalb, **was** gefragt ist und **wer** es liefert, und nicht, wie der Satz lauten soll
- Reine Umformulierungen

Der zweite Punkt ist eine bewusste Entscheidung und kein Versehen.

## Was hier nicht wiederholt wird

Die Einstufung, die Rollenfrage im Detail und die Audit-Vorbereitung haben eigene Repositories. Dieses verweist darauf; das [Repository-Netz](./docs/repository-network.md) zeigt, wohin ein Beitrag gehört.

## Vorgehen

Kleine Korrekturen gern direkt als Pull Request. Bei größeren Änderungen vorher ein Issue.

`npm run validate` prüft, dass alle Pflichtpfade vorhanden und die JSON-Dateien lesbar sind. Die Prüfung läuft auch in CI.

## Rechtliches

Beiträge stehen unter der MIT-Lizenz dieses Repositories. Inhalte hier sind keine Rechtsberatung; wer eine Fundstelle ändert, gibt bitte die Quelle an.

Keine echten Systemdaten in Beispielen. Ein Anbietername zusammen mit einem dokumentierten Mangel gehört nicht in ein öffentliches Repository.

## Kodierung

Alle Dateien sind UTF-8. Das klingt selbstverständlich, war es in diesem Repository aber eine Weile nicht — deutsche Umlaute erschienen auf GitHub als Ersatzzeichen. Wer unter Windows arbeitet, prüft das vor dem Commit.
