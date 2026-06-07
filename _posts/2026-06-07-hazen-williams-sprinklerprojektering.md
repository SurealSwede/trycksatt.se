---
layout: post
title: "Hazen-Williams i sprinklerprojektering"
date: 2026-06-07
kategori: Hydraulik
lasttid: 6
ingress: Hazen-Williams-ekvationen är grunden för all hydraulisk beräkning av sprinklersystem. Här förklaras formeln, parametrarna och hur du tolkar resultaten i praktiken.
---

## Vad är Hazen-Williams?

Hazen-Williams är en empirisk formel för att beräkna tryckfall i vätsketransporterande rör. Den är den dominerande beräkningsmetoden inom sprinklerteknik och används som standard i både **SBF 120** och **EN 12845**.

Formeln är förenklad jämfört med Darcy-Weisbach — den tar inte hänsyn till vätskans viskositet utan förutsätter att vatten vid normala temperaturer transporteras.

## Formeln

```
Pf = (6.05 × 10⁵ × Q^1.85) / (C^1.85 × d^4.87) × L
```

### Parametrar

| Symbol | Enhet | Beskrivning |
|--------|-------|-------------|
| Pf | bar | Tryckfall |
| Q | l/min | Flöde |
| C | — | Hazen-Williams C-faktor |
| d | mm | Innerdiameter |
| L | m | Totallängd (fysisk + ekvivalent) |

## C-faktorn

C-faktorn representerar rörledningens inre ytjämnhet. Ett högt C-värde innebär lägre friktion och därmed lägre tryckfall.

| Rörtyp | C-faktor |
|--------|----------|
| Handelstub (svartrörs) | 120 |
| Lättviktsrör | 130 |
| Gängrör | 120 |
| Rostfria STH100 | 140 |

**Viktigt:** C=120 används som standardvärde för ekvivalenta rörlängder i Tabell 23, SBF 120 — oavsett vilken rörtyp som faktiskt används.

## Ekvivalenta rörlängder

Armatur (böjar, T-rör, ventiler) genererar tryckfall precis som rak rörledning. För att förenkla beräkningen omvandlas armaturen till en *ekvivalent rörlängd* — hur lång rak rörledning som ger samma tryckfall.

Tabell 23 i SBF 120 ger standardvärden per DN för de vanligaste armaturerna:

| DN | 90° vinkel | T-rör (genomflöde) |
|----|-----------|---------------------|
| 25 | 0,77 m | 1,50 m |
| 40 | 1,20 m | 2,40 m |
| 50 | 1,50 m | 2,90 m |
| 65 | 1,90 m | 3,80 m |
| 100 | 3,00 m | 6,10 m |

Den totala beräkningslängden är:

```
L_tot = L_fysisk + (antal_böjar × ekvivalent_böj) + (antal_T-rör × ekvivalent_T)
```

## Praktisk tolkning

### Tryckfall per meter

Det är användbart att normalisera tryckfallet till bar per meter — det ger en omedelbar känsla för om dimensioneringen är rimlig.


### Hastighetsbegränsning

SBF 120 anger normalt max **6 m/s** för ventiler och **10 m/s** som absolut maximum för rörledningar. Hög hastighet genererar oljud och ökad erosion.

För given diameter ger hastighetsgränsen ett maximalt flöde:

```
Qmax = π × (d/2)² × v_max × 60 000
```

## Beräkna med verktyget

Alla beräkningar i den här artikeln kan du utföra direkt i det [hydrauliska beräkningsverktyget](/verktyg/) — välj rörtyp, mata in flöde och antal armaturdelar, så räknar verktyget ut tryckfall och hastighet automatiskt.

---

*Formlerna i denna artikel är hämtade från SBF 120 (SBF 2016:2) och EN 12845. Kontrollera alltid mot aktuell norm.*
