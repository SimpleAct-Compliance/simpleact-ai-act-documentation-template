# Vorlage: Dokumentationsprüfung

Nicht „ist jeder Abschnitt gefüllt", sondern: **ist das vorzeigbar?**

**System:** ___  **Version:** ___  **Geprüft am:** ___  **Geprüft durch:** ___ (nicht der Dokumentationsverantwortliche)

---

## 1 Grundlage

- [ ] Die **Rolle** ist bestimmt und begründet: Anbieter oder Betreiber
- [ ] **Art. 25 geprüft**, mit Datum — auch wenn das Ergebnis Nein lautet
- [ ] Die Hochrisiko-Einstufung liegt vor, mit Anhangbezug samt Nummer
- [ ] Bei Berufung auf **Art. 6 Abs. 3**: die Bewertung ist dokumentiert, und die Profiling-Frage ist beantwortet
- [ ] Die dokumentierte Version **stimmt mit der laufenden überein** — oder die Abweichung ist vermerkt

Der letzte Punkt ist der, der in Prüfungen am schnellsten auffällt.

## 2 Die vier nicht nachholbaren Abschnitte

- [ ] **Entwurfsentscheidungen** mit Datum, Alternativen und Begründung — nicht rekonstruiert
- [ ] **Datenquellentabelle** je Quelle, mit Rechtsgrundlage und Bereinigungsschritten
- [ ] Datenquellentabelle enthält die Spalte **bekannte Verzerrungen**, und sie ist nicht leer
- [ ] **Testprotokolle je Version**, datiert, mit Datensatz-Kennung — als Reihe, nicht als Einzelstück
- [ ] **Änderungstabelle** lückenlos ab einem benannten Datum
- [ ] Änderungstabelle enthält die Spalte zur **Wesentlichkeit nach Art. 3 Nr. 23**
- [ ] Änderungstabelle enthält auch **Modellwechsel bei Fremdbestandteilen**

Wo einer dieser Abschnitte nur ab einem bestimmten Datum geführt wird: Ist dieser Beginn als **benannte Lücke** dokumentiert, statt den Zeitraum davor zu rekonstruieren?

## 3 Inhaltliche Tiefe

- [ ] Die **Zweckbestimmung** ist eng gefasst, nicht breit
- [ ] Der Abschnitt **Grenzen** benennt, was das System nicht leistet — konkret, nicht als Floskel
- [ ] Die **vorhersehbare Fehlanwendung** ist benannt und nicht leer
- [ ] Die **Annahmen** aus der Einstufung sind als Grenzen übernommen
- [ ] Genauigkeit und Robustheit sind mit **Messwerten** und Datensatzbezug angegeben, nicht beschrieben
- [ ] Zum Restrisiko steht da, **warum es vertretbar ist**
- [ ] Die Betriebsanleitung sagt, **woran eine falsche Ausgabe erkennbar ist**

Der letzte Punkt entscheidet darüber, ob die menschliche Aufsicht beim Betreiber überhaupt funktionieren kann.

## 4 Menschliche Aufsicht

- [ ] Beschrieben ist, wie das System Aufsicht technisch **ermöglicht**
- [ ] Beschrieben ist, wie es **angehalten** werden kann
- [ ] **Nachweis aus dem Betrieb:** Zahl der geänderten oder verworfenen Ausgaben je Monat liegt vor
- [ ] Diese Zahl wurde mit der Vorperiode verglichen

Ohne die Betriebszahl belegt der Abschnitt nur, dass Aufsicht möglich ist — nicht, dass sie stattfindet.

## 5 Fremdbestandteile

- [ ] Je Fremdbestandteil: Anbieter, Modell, **Version**
- [ ] Dokumentiert, **welche Angaben der Anbieter nicht liefert**, mit Datum der Anfrage
- [ ] Geprüft, ob der Anbieter seine GPAI-Pflichten erfüllt und die Unterlagen bereitstellt
- [ ] Ein **Testsatz** gegen den stillen Modellwechsel läuft, mit Turnus

## 6 Nachweise

- [ ] Je Abschnitt ist der zugehörige **Nachweis benannt**, nicht nur der Inhalt beschrieben
- [ ] Je Nachweis: **Version**, Datum, Fundort, Urheber
- [ ] Je Nachweis ein Zustand: offen / erbracht / geprüft / freigegeben
- [ ] Nachweise, die durch eine neue Version ungültig wurden, sind **zurück auf offen** gesetzt
- [ ] **Probe durchgeführt:** einen Nachweis angefordert, Zeit gemessen: ___

Die Probe ist in zehn Minuten gemacht und sagt mehr als jede Vollständigkeitszählung. Dauert es länger als eine Stunde, ist der Nachweis in einer echten Prüfung nicht vorlegbar.

## 7 Lücken

- [ ] Fehlende Abschnitte sind als **benannte Lücke** geführt, mit Grund, Person und Termin
- [ ] Kein Abschnitt ist mit Füllsätzen überdeckt
- [ ] Bei jeder Lücke steht, **warum** sie besteht — Anbieter liefert nicht, noch nicht gemessen, noch nicht entschieden

Füllsätze fallen auf und stellen den Rest in Frage: Wer einen Abschnitt erkennbar mit Worten gefüllt hat, hat möglicherweise mehrere so gefüllt.

## 8 Zuständigkeit und Freigabe

- [ ] Je Abschnitt ist ein **Name** eingetragen, der ihn geliefert hat
- [ ] **Geprüft** hat jemand anderes als der Dokumentationsverantwortliche
- [ ] Die Freigabe ist auf eine **Version** bezogen
- [ ] Offene Punkte bei Freigabe sind als Zahl vermerkt
- [ ] Frühere Fassungen bleiben erhalten

## 9 Verzahnung

- [ ] Verweis ins **Verarbeitungsverzeichnis** (Art. 30 DSGVO), sofern personenbezogene Daten
- [ ] Geprüft, ob eine **DSFA** nach Art. 35 DSGVO erforderlich ist
- [ ] Bei Hochrisiko geprüft, ob eine **Grundrechte-Folgenabschätzung** nach Art. 27 AI Act erforderlich ist
- [ ] Verweis auf den **Plan nach Art. 72** und die vorliegenden Berichte
- [ ] Verweis auf den Inventareintrag und den Einstufungsbogen
- [ ] Angaben werden nicht doppelt geführt

---

## Befunde

| # | Befund | Abschnitt | Verantwortlich (Person) | Termin |
|---|---|---|---|---|
| | | | | |

## Ergebnis

- [ ] **Vorzeigbar** — offene Punkte sind benannt und terminiert
- [ ] **Nicht vorzeigbar** — Begründung: ___
- [ ] **Neufassung erforderlich** — Verantwortlich: ___ Termin: ___

**Geprüft durch:** ___  **Datum:** ___  **Nächste Prüfung:** ___

## Weiter

[Vorlage](./technical-documentation-template.md) · [Die Nachweisschicht](../knowledge-base/eu-ai-act/evidence-layer.md) · [Audit-Vorbereitung](https://github.com/SimpleAct-Compliance/simpleact-ai-audit-readiness)
