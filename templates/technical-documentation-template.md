# Vorlage: Technische Dokumentation (Anhang IV)

Gliederung nach Anhang IV der Verordnung (EU) 2024/1689. Je Abschnitt steht, **was gefragt ist**, **wer das liefert** und **welcher Nachweis dazugehört**.

Pflicht für **Anbieter** von Hochrisikosystemen (Art. 11). Wenn Sie unsicher sind, ob Sie Anbieter sind: [Wer dokumentieren muss](../knowledge-base/eu-ai-act/scope-and-actors.md).

**Lücken werden benannt, nicht gefüllt.** Ein Abschnitt mit „liegt nicht vor, verantwortlich ___, Termin ___" ist besser als einer mit Füllsätzen.

---

## Kopf

| Feld | Eintrag |
|---|---|
| System | |
| **Version** | |
| Zweckbestimmung (ein Satz) | |
| Anbieter | |
| Dokumentationsverantwortlicher | |
| Stand dieser Fassung | |
| Vorherige Fassung | |

---

## 1 Allgemeine Beschreibung

**Liefert:** Produkt oder Fachbereich

| Angabe | Eintrag |
|---|---|
| Zweckbestimmung, einschließlich Nutzungskontext | |
| Name und Kontakt des Anbieters | |
| Version und wie sie im System ablesbar ist | |
| Vorgesehene Betreiber und Nutzergruppen | |
| Form der Bereitstellung (Software, eingebettet, als Dienst) | |
| Hardware, auf der es läuft | |
| Beschreibung der Benutzerschnittstellen | |
| Betriebsanleitung für Betreiber — Fundort | |

**Hinweis zur Zweckbestimmung:** eng fassen. Was Sie hier als vorgesehene Verwendung beschreiben, müssen Sie auch bewerten, testen und dokumentieren.

**Zur Betriebsanleitung:** Sie ist nicht Nebenprodukt, sondern Teil des Produkts. Betreiber erfüllen damit ihre Pflichten nach Art. 26. Was hineingehört und oft fehlt: die Grenzen, die vorhersehbaren Fehlerarten mit Beispielen, was ein Betreiber nicht damit tun darf, und woran eine falsche Ausgabe erkennbar ist.

---

## 2 Entwicklung und Verfahren

**Liefert:** Entwicklung, Datenschutz, Qualitätssicherung

### 2.1 Entwicklungsschritte und Fremdbestandteile

| Angabe | Eintrag |
|---|---|
| Entwicklungsschritte | |
| Verwendete Fremdbestandteile, vortrainierte Modelle | |
| Je Fremdbestandteil: Anbieter, Modell, **Version** | |
| **Welche Angaben der Anbieter nicht liefert** — mit Datum der Anfrage | |

Die letzte Zeile ist wichtig: Eine dokumentierte Anbieterlücke ist ein Befund gegen den Anbieter. Dieselbe Lücke ohne Dokumentation ist ein Befund gegen Sie.

### 2.2 Entwurfsentscheidungen

| Datum | Entscheidung | Alternativen | Begründung | Durch |
|---|---|---|---|---|
| | | | | |

**Dieser Abschnitt ist nicht nachholbar.** Nach zwei Jahren weiß niemand mehr, welche Alternative verworfen wurde und warum. Vier Sätze je Entscheidung genügen — aber sie müssen zum Zeitpunkt der Entscheidung entstehen.

Dazu gehören auch die **Annahmen über die Personen**, auf die das System angewandt wird.

### 2.3 Systemarchitektur und Ressourcen

| Angabe | Eintrag |
|---|---|
| Architektur, Zusammenwirken der Komponenten | |
| Rechenressourcen | |

### 2.4 Daten

Je Datenquelle eine Zeile. **Nicht nachholbar.**

| Quelle | Zeitraum | Umfang | Beschaffung | Rechtsgrundlage | Bereinigung | Bekannte Verzerrungen |
|---|---|---|---|---|---|---|
| | | | | | | |

Die letzte Spalte ist die unangenehme und die wertvollste. Eine dokumentierte Verzerrung ist ein Nachweis von Sorgfalt; dieselbe Verzerrung, die später auffällt, ist ein Befund.

### 2.5 Menschliche Aufsicht

| Angabe | Eintrag |
|---|---|
| Wie das System Aufsicht technisch **ermöglicht** | |
| Welche Schnittstellen dafür vorgesehen sind | |
| Woran eine falsche Ausgabe erkennbar ist | |
| Wie das System angehalten werden kann | |
| **Nachweis aus dem Betrieb:** geänderte oder verworfene Ausgaben je Monat | |

Die letzte Zeile ist der einzige Nachweis dafür, dass Aufsicht tatsächlich ausgeübt wird. Alles darüber belegt nur, dass sie möglich ist.

### 2.6 Validierung und Test

Je Version ein Protokoll. **Nicht nachholbar.**

| Datum | Version | Verfahren | Metrik | Ergebnis | Testdatensatz-Kennung | Durch |
|---|---|---|---|---|---|---|
| | | | | | | |

Die **Reihe** ist der Nachweis, nicht der letzte Lauf.

---

## 3 Überwachung, Funktionsweise, Kontrolle

**Liefert:** Entwicklung, IT-Sicherheit, Fachbereich

| Angabe | Eintrag |
|---|---|
| Genauigkeit, mit Messwert und Datensatz | |
| Robustheit, mit Messwert | |
| Cybersicherheit, Prüfbericht | |
| Vorhersehbare unbeabsichtigte Ergebnisse | |
| Risikoquellen für Gesundheit, Sicherheit, Grundrechte | |
| **Grenzen: was das System nicht leistet** | |
| Spezifikationen der Eingabedaten | |
| Angaben, die Betreiber zur Auslegung der Ausgaben brauchen | |

**Zum Abschnitt Grenzen:** Er wird oft zu knapp gehalten und ist der Teil, auf den sich Betreiber verlassen — und der Teil, der in einem Vorfall gelesen wird. Was bei der Einstufung als **Annahme** festgehalten wurde, gehört hier als Grenze hinein.

---

## 4 Risikomanagementsystem (Art. 9)

**Liefert:** Compliance, mit Zuarbeit

| Risiko | Bewertung | Maßnahme | Restrisiko | Warum vertretbar | Datum |
|---|---|---|---|---|---|
| | | | | | |

Die Spalte „warum vertretbar" ist die, auf die es ankommt. Ein Restrisiko ohne Begründung ist eine Feststellung, keine Bewertung.

---

## 5 Änderungen am Lebenszyklus

**Liefert:** Entwicklung, laufend. **Nicht nachholbar.**

| Datum | Version | Änderung | Wesentlich nach Art. 3 Nr. 23? | Begründung | Folge | Durch |
|---|---|---|---|---|---|---|
| | | | | | | |

**Der praktisch wichtigste Teil der ganzen Dokumentation.** Er beantwortet die Frage, die jede Prüfung stellt: Welcher Stand war zu welchem Zeitpunkt in Betrieb? Ohne ihn lässt sich kein anderer Nachweis zeitlich zuordnen.

Die Spalte zur Wesentlichkeit zwingt dazu, die Rollenfrage bei jeder Änderung zu stellen statt einmal im Jahr: Wer wesentlich ändert, kann nach Art. 25 zum Anbieter werden.

**Auch eintragen:** Modellwechsel bei Fremdbestandteilen. Wenn die eigene Version gleich bleibt, der Zulieferer aber getauscht hat, ist das System ein anderes.

---

## 6 Angewandte Normen

| Norm | Fassung | Abschnitt | Angewandt |
|---|---|---|---|
| | | | |

Wo keine harmonisierte Norm angewandt wurde: Beschreibung der stattdessen getroffenen Lösungen, und warum sie die Anforderung erfüllen.

---

## 7 EU-Konformitätserklärung

| Feld | Eintrag |
|---|---|
| Fundort der Erklärung | |
| Datum | |
| Unterzeichner | |
| Bezug auf Version | |

---

## 8 Beobachtung nach dem Inverkehrbringen (Art. 72)

| Feld | Eintrag |
|---|---|
| Fundort des Plans | |
| Vorliegende Berichte, Zeitraum | |
| Letzte Auswertung | |

Die **Reihe** der Berichte ist der Nachweis. Ein einzelner aktueller Bericht kann am Vortag der Prüfung entstanden sein.

---

## Offene Punkte

| Abschnitt | Was fehlt | Warum | Verantwortlich (Person) | Termin |
|---|---|---|---|---|
| | | | | |

Die Spalte „warum" unterscheidet eine erkannte Lücke von einer vergessenen. „Anbieter liefert die Trainingsdatenherkunft nicht, angefragt am 12.9.2026" ist eine erkannte Lücke.

## Freigabe

| Feld | Eintrag |
|---|---|
| Zusammengestellt durch | |
| Geprüft durch (andere Person) | |
| Freigegeben durch | |
| Für Version | |
| Datum | |
| Offene Punkte bei Freigabe | Anzahl |

Frühere Fassungen bleiben erhalten. In einer Prüfung lautet die Frage, was zu einem bestimmten Zeitpunkt dokumentiert war.
