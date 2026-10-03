# Das Netz der Repositories

Dieses Repository deckt den **Dokumentationsschritt** ab. Es setzt eine Einstufung und eine geklärte Rollenfrage voraus.

## Der Weg

```
  Inventar -> Einstufung -> Prüfung -> [Dokumentation] -> Audit -> Betrieb
```

| Richtung | Repository | Beantwortet |
|---|---|---|
| vorher | [Risikoeinstufung](https://github.com/SimpleAct-Compliance/simpleact-ai-risk-classification-eu) | Ist es Hochrisiko? Greift Anhang IV überhaupt? |
| vorher | [AI Act für SaaS](https://github.com/SimpleAct-Compliance/simpleact-ai-act-for-saas) | Sind wir Anbieter? |
| vorher | [KI-Inventar](https://github.com/SimpleAct-Compliance/simpleact-ai-system-inventory) | woher die Grundangaben kommen |
| vorher | [Anbieterregister](https://github.com/SimpleAct-Compliance/simpleact-model-vendor-register) | welche Angaben der Modellanbieter liefert |
| daneben | [Prüfliste AI Act](https://github.com/SimpleAct-Compliance/simpleact-ai-act-checklist) | die Nachweiszustände, ausführlich |
| daneben | [Vorlagensammlung](https://github.com/SimpleAct-Compliance/simpleact-ai-act-templates) | Vorlagen für die übrigen Nachweise |
| danach | [Audit-Vorbereitung](https://github.com/SimpleAct-Compliance/simpleact-ai-audit-readiness) | wenn eine Prüfung von außen ansteht |
| danach | [Vorfallmanagement](https://github.com/SimpleAct-Compliance/simpleact-incident-management) | Art. 72 und 73, Abschnitt 8 von Anhang IV |

Die zwei ersten Zeilen sind nicht optional. Wer mit der Dokumentation beginnt, ohne die Rollenfrage geklärt zu haben, schreibt möglicherweise etwas, das er nicht schuldet — oder lässt etwas weg, das er schuldet.

## Besonders: das Anbieterregister

Bei Fremdbestandteilen hängt die eigene Dokumentation an den Angaben des Modellanbieters. Vier Abschnitte sind ohne ihn nicht füllbar: Trainingsdatenherkunft, Entwurfsentscheidungen des Modells, Genauigkeitsangaben der Grundkomponente, Modellversion und deren Änderungsverlauf.

Deshalb gehören die Beschaffungsfragen **vor** den Vertrag, nicht in die Dokumentationsphase. Das [Anbieterregister](https://github.com/SimpleAct-Compliance/simpleact-model-vendor-register) enthält sie.

## Übergreifend

| Repository | Wofür |
|---|---|
| [Governance-Rahmenwerk](https://github.com/SimpleAct-Compliance/simpleact-ai-governance-framework) | wie alle Teile zusammenhängen |
| [Governance-Playbook](https://github.com/SimpleAct-Compliance/simpleact-ai-governance-playbook) | wer liefert, wer prüft, wer gibt frei |
| [KI-Kompetenz](https://github.com/SimpleAct-Compliance/elearning) | Art. 4, und die Grundlage dafür, dass Aufsicht funktioniert |
| [Integrationen](https://github.com/SimpleAct-Compliance/simpleact-integrations-apis) | Änderungsverlauf dort führen, wo Änderungen stattfinden |

Das letzte ist für dieses Repository praktisch relevant: Ein Änderungsverlauf, der an einer anderen Stelle gepflegt werden muss als die Änderung selbst, wird nicht gepflegt.

## Datenschutzseite

| Repository | Berührung zu Anhang IV |
|---|---|
| [DSGVO-Grundlagen](https://github.com/SimpleAct-Compliance/simpleact-gdpr-compliance-workspace) | Art. 30, Rechtsgrundlage für die Datenquellentabelle |
| [DSFA und FRIA](https://github.com/SimpleAct-Compliance/simpleact-dpia-dsfa-workflow) | Art. 35 DSGVO und Art. 27 AI Act; teilweise deckungsgleiche Risikobetrachtung |
| [Datenschutzverletzungen](https://github.com/SimpleAct-Compliance/simpleact-gdpr-data-breach-management) | Art. 33 und 34, neben Art. 73 AI Act |

Die Datenquellentabelle in Abschnitt 2 und das Verarbeitungsverzeichnis greifen auf dieselben Angaben zu. Wer beides getrennt erhebt, macht die Arbeit zweimal und hat nach einem halben Jahr an einer von beiden Stellen veraltete Angaben.

## Tarifgenaue Anbieterangaben

Für die Abschnitte zu Fremdbestandteilen: ein öffentliches Register mit tarifgenauen Angaben einzelner KI-Werkzeuge, jede mit Quelle und Prüfdatum — **[actcomp.de](https://actcomp.de)**
