---
layout: artikel
title: "Hazen-Williams förklarad för sprinklerprojektörer"
date: 2026-06-07
tags: [Hydraulik]
description: "Formeln bakom tryckfallsberäkningar i sprinklersystem — vad C-faktorn betyder och hur du väljer rätt rörtyp."
---

Hazen-Williams är den formel som används för att beräkna tryckfall i vattenledningar med fullt turbulent flöde — vilket är precis det vi har i sprinklersystem.

## Formeln

```
Pf = (6.05 × 10⁵ × Q^1.85) / (C^1.85 × d^4.87) × L
```

Där:

| Symbol | Enhet | Beskrivning |
|--------|-------|-------------|
| Pf | bar | Tryckfall |
| Q | l/min | Flöde |
| C | — | Hazen-Williams C-faktor |
| d | mm | Innerdiameter |
| L | m | Totallängd inkl. ekvivalenter |

## C-faktorns betydelse

C-faktorn beskriver rörytans jämnhet. Högre C = jämnare rör = lägre friktion:

| Rörtyp | C-faktor |
|--------|----------|
| Handelstub (EN 10217-1) | 120 |
| Lättviktsrör | 130 |
| Gängrör (SS-EN 10255) | 120 |
| Rostfria rör (1.4404) | 140 |

SBF 120 använder **C = 120** som standardvärde för ekvivalenta rörlängder i Tabell 23.

## Ekvivalenta rörlängder

Armatur (böjar, T-rör) räknas om till ekvivalenta rörlängder och adderas till den fysiska rörlängden:

```
L_tot = L_fysisk + (böjar × L_böj) + (T-rör × L_T)
```

Värdena hämtas ur **Tabell 23 i SBF 120**.

> Prova beräkningarna direkt i [hydraulikverktyget](/verktyg/).
