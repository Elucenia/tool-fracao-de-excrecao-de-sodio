<!-- ELUCENIA technical documentation · fracao-de-excrecao-de-sodio · de · no clinical/professional/rights approval -->

# Fraktionelle Natriumausscheidung (FENa)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/fracao-de-excrecao-de-sodio)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Urinnatrium

`una`

mEq/L · Bereich: 1–300

### Serumnatrium

`pna`

mEq/L · Bereich: 100–180

### Urinkreatinin

`ucr`

mg/dL · Bereich: 1–500

### Serumkreatinin

`pcr`

mg/dL · Bereich: 0,2–20

### Diuretikaeinnahme in den letzten 24 h?

`diuretico`

- `0` — Nein
- `1` — Ja

## Fassung der Methode

FENa/Espinel 1976; Miller 1978, 100×UNa×PCr/(PNa×UCr); gleichzeitige Proben

## Dokumentierte Formel

FENa (%) = (Urin-Na × Serumkreatinin) ÷ (Serum-Na × Urinkreatinin) × 100.

Möglichst gleichzeitig entnommene Urin- und Blutproben vor Diuretika oder Volumengabe verwenden.

## Grenzen und Population

Die Evidenz von Miller 1978 bezieht sich auf akute Oligurie und zeigte, dass Urinindizes prärenale Ursachen nicht immer von Tubulusnekrose unterscheiden. Das Ergebnis allein bestimmt die Ursache der Nierenfunktionsstörung nicht. Klinische Bedingungen, Probenzeitpunkte und Medikamente müssen entsprechend der Quelle der verwendeten Version berücksichtigt werden.

## Referenzen

- [Miller TR et al. Urinary diagnostic indices in acute renal failure: a prospective study. Ann Intern Med, 1978.](https://doi.org/10.7326/0003-4819-89-1-47)

- [Espinel CH. The FENa test: use in the differential diagnosis of acute renal failure. JAMA, 1976.](https://doi.org/10.1001/jama.1976.03270060029022)

- [Steiner RW. Interpreting the fractional excretion of sodium. Am J Med, 1984.](https://doi.org/10.1016/0002-9343(84)90368-1)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

FENa < 1 %: spricht für prärenale Azotämie (Tubulus erhalten, Natriumretention)


### 2

FENa zwischen 1 und 2 %: Zwischenbereich, im klinischen Kontext interpretieren


### 3

FENa > 2 %: spricht für akute Tubulusnekrose (intrinsische Nierenschädigung)

Bei Diuretika in den letzten 24 h steigt die FENa auch im prärenalen Zustand an: bevorzugen Sie die fraktionelle Harnstoffexkretion.

