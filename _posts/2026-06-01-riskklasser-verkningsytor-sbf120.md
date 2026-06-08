---
layout: post
title: "Riskklasser och verkningsytor i SBF 120"
date: 2026-06-01
kategori: Normer
lasttid: 4
ingress: OH1 till HHP3 — vad innebär riskklasserna i SBF 120 och hur påverkar de dimensioneringen av ett sprinklersystem?
---

## Bakgrund

Sprinklersystem dimensioneras utifrån den verksamhet som ska skyddas. SBF 120 delar in riskerna i klasser som styr vattentäthet, verkningsyta och minsta flöde.

## Riskklassöversikt

| Riskklass | Vattentäthet | Verkningsyta (vått) | Verkningsyta (torrt) |
|-----------|-------------|---------------------|----------------------|
| OH1 | 5 mm/min | 72 m² | 90 m² |
| OH2 | 5 mm/min | 144 m² | 180 m² |
| OH3 | 5 mm/min | 216 m² | 270 m² |
| OH4 | 5 mm/min | 360 m² | Ej tillåtet |
| HHP1 | 7,5 mm/min | 260 m² | 325 m² |
| HHP2 | 10 mm/min | 260 m² | 325 m² |
| HHP3 | 12,5 mm/min | 260 m² | 325 m² |

*Källa: Tabell i SBF 120 (SBF 2016:2)*

## Minsta teoretiska flöde

Minsta teoretiska beräkningsflöde för ett system ges av:

```
Q_min = vattentäthet (mm/min) × verkningsyta (m²)
```

Enhetskonverteringen stämmer direkt: 1 mm/min × 1 m² = 1 l/min.

### Exempel: OH1

```
Q = 5 mm/min × 72 m² = 360 l/min
```

### Exempel: HHP2

```
Q = 10 mm/min × 260 m² = 2 600 l/min
```

Skillnaden illustrerar tydligt varför pumpdimensionering för HHP är ett helt annat projekt än för OH1.

## Torra kontra våta system

Torrörssystem har en fördröjd vattenutsläppning eftersom rörsystemet måste trycktömmas på luft först. Normen kompenserar för detta med en ökad verkningsyta — typiskt 25 % mer än för vätrörsystem.

OH4 är inte tillåtet som torrörssystem alls, vilket speglar att de höga flödena kombinerat med fördröjd aktivering skulle ge oacceptabla brandskador.

---

*Artikeln baseras på SBF 120 (SBF 2016:2). Kontrollera alltid mot aktuell version av normen.*
