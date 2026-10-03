# Technische Dokumentation nach Anhang IV

**Das meiste davon lässt sich nicht nachträglich schreiben.** Entwurfsentscheidungen, Testergebnisse, Datenherkunft — das sind Dinge, die während der Entwicklung festgehalten werden oder gar nicht. Dieses Repository beschreibt, was Anhang IV verlangt, in welcher Form, und welche Abschnitte laufend mitgeführt werden müssen.

*What Annex IV actually asks for, section by section, and which parts cannot be reconstructed after the fact.*

---

## Wen es betrifft

Die technische Dokumentation nach **Art. 11 in Verbindung mit Anhang IV** ist eine **Anbieterpflicht** für Hochrisikosysteme. Betreiber brauchen sie nicht.

Der Haken: Nach **Art. 25** kann ein Betreiber zum Anbieter werden — am häufigsten durch den Fall, der ohne Anlass eintritt: ein allgemeines Werkzeug, eingesetzt in einem Anhang-III-Bereich. Wer ein Sprachmodell Bewerbungen vorsortieren lässt, kann Anbieter eines Hochrisikosystems sein, ohne es geplant zu haben.

Bevor Sie hier weiterlesen, ist deshalb eine Frage zu klären: **Sind Sie Anbieter?** Dazu: [Wer dokumentieren muss](./knowledge-base/eu-ai-act/scope-and-actors.md)

## Die Fristen

Nach dem **Digital Omnibus** (Verordnung (EU) 2026/1744, in Kraft seit 27.7.2026):

| Hochrisiko nach | Anwendbar ab |
|---|---|
| Anhang III | **2.12.2027** — um 16 Monate verschoben |
| Anhang I | 2.8.2028 |

Das klingt nach Zeit und ist es nur teilweise: Die Abschnitte, die laufend entstehen müssen, entstehen nicht rückwirkend. Siehe unten.

## Was sich nicht nachträglich schreiben lässt

| Abschnitt | Warum nicht |
|---|---|
| **Entwurfsentscheidungen mit Begründung** | nach zwei Jahren weiß niemand mehr, welche Alternative verworfen wurde und warum |
| **Datenherkunft und Aufbereitung** | welche Quelle wann wie bereinigt wurde, steht in keinem Repository |
| **Validierung und Testergebnisse** | Tests lassen sich wiederholen, die Ergebnisse der damaligen Version nicht |
| **Änderungsverlauf** | welcher Stand wann in Betrieb war, ist die Frage jeder Prüfung |

Diese vier sind der Grund, warum eine nachträgliche Dokumentation teuer ist — und warum sie an den Stellen Lücken hat, die in einer Prüfung auffallen.

Die anderen Abschnitte — allgemeine Beschreibung, Normen, Konformitätserklärung — sind Schreibarbeit und jederzeit nachholbar.

Ausführlich: [Was laufend entstehen muss](./knowledge-base/eu-ai-act/documentation-logic.md)

## Die Frage, die jede Prüfung stellt

> **Welcher Stand war zu welchem Zeitpunkt in Betrieb?**

Darauf läuft die technische Dokumentation hinaus. Ein Nachweis ohne Versionsbezug belegt einen Zeitpunkt, nicht einen Zustand — und der Änderungsverlauf nach Anhang IV Nr. 5 ist der praktisch wichtigste Teil der ganzen Dokumentation, obwohl er wie Buchhaltung aussieht.

## Lücken benennen, nicht füllen

Ein Abschnitt mit „liegt nicht vor, verantwortlich ___, Termin ___" ist in einer Prüfung besser als ein Abschnitt mit Füllsätzen. Füllsätze fallen auf und stellen den Rest in Frage: Wer einen Abschnitt erkennbar mit Worten gefüllt hat, hat möglicherweise mehrere so gefüllt.

## Inhalt

| Dokument | Inhalt |
|---|---|
| [Was wann gilt](./knowledge-base/eu-ai-act/overview.md) | Fristen, und warum die Verschiebung weniger Zeit verschafft als es aussieht |
| [Begriffe](./knowledge-base/eu-ai-act/definitions.md) | Zweckbestimmung, wesentliche Änderung, Version |
| [Wer dokumentieren muss](./knowledge-base/eu-ai-act/scope-and-actors.md) | Anbieterpflicht, und der Weg dorthin über Art. 25 |
| [Wann Anhang IV greift](./knowledge-base/eu-ai-act/risk-logic.md) | Hochrisiko, und was bei anderen Klassen zu dokumentieren ist |
| [Was laufend entstehen muss](./knowledge-base/eu-ai-act/documentation-logic.md) | die vier nicht nachholbaren Abschnitte |
| [Die Nachweisschicht](./knowledge-base/eu-ai-act/evidence-layer.md) | wie Dokumentation und Nachweise zusammenhängen |
| [Woher die Angaben kommen](./knowledge-base/eu-ai-act/inventory-and-governance.md) | Inventar, Anbieterangaben, Zuständigkeit |

### Vorlagen

| Vorlage | Zweck |
|---|---|
| [Technische Dokumentation](./templates/technical-documentation-template.md) | Anhang IV, Abschnitt für Abschnitt, mit Hinweisen je Abschnitt |
| [Dokumentationsprüfung](./templates/documentation-checklist.md) | ist das vorzeigbar? |

Maschinenlesbar: [framework/simpleact-framework.json](./framework/simpleact-framework.json) · [llms.txt](./llms.txt)

## Davor und danach

- vorher: [Risikoeinstufung](https://github.com/SimpleAct-Compliance/simpleact-ai-risk-classification-eu) — ob Anhang IV überhaupt greift
- vorher: [AI Act für SaaS](https://github.com/SimpleAct-Compliance/simpleact-ai-act-for-saas) — wenn die Anbieterfrage offen ist
- daneben: [Vorlagensammlung](https://github.com/SimpleAct-Compliance/simpleact-ai-act-templates) — Vorlagen für die übrigen Nachweise
- danach: [Audit-Vorbereitung](https://github.com/SimpleAct-Compliance/simpleact-ai-audit-readiness) — wenn eine Prüfung ansteht

## In Software umsetzen

[SimpleAct](https://simpleact.de) führt die Anhang-IV-Dokumentation vorlagengestützt mit verknüpften Nachweisen, Freigabeläufen und Änderungsverlauf: **[AI Act Software](https://simpleact.de/ai-act-software)**

## Stand und Lizenz

Zuletzt aktualisiert: 2026-10-03 · MIT — frei nutzbar, auch kommerziell. Keine Rechtsberatung.
