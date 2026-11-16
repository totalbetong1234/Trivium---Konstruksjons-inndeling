# TB Betong Trivium – Trimble Connect extension (1307 Trivium)

Oversikt over betongkonstruksjonene i Trivium RIB-modellen (Total Betong).

## Installasjon
Prosjekt → **Innstillinger** → **Extensions** → **+ Add Custom** →
`https://totalbetong1234.github.io/Trivium---Konstruksjons-inndeling/manifest.json`

## Grupper (sortert på Revit-familie og Type)
| Gruppe | Innhold |
|---|---|
| Fundamenter | Punktfundamenter («Betong A×B×C», også de med lange beskrivende navn), Pelehode 600 |
| Kran | Kranfundament |
| Magerbetong | All Type «Magerbetong» (fundamentplater, fundamenter, Slab Edge – Slab Edge har ikke volum) |
| Bunnplate/dekker | Floor: Betongdekke 300/400 mm |
| Påstøp og gulv | Floor: Påstøp 80/100 mm, Gulv på grunn 120 mm |
| Grunnmur | Grunnmur Betong 200 |
| Yttervegger | YV Betong … |
| Innervegger | IV Betong … og Pilaster |
| Søyler | Plasstøpte søyler |
| Bjelker | Plasstøpte bjelker |
| Kumringer | Kumring DN 1000 / DN 650 (ingen volum i modellen) |
| **Stål** | Stålsøyler, stålplater – holdes utenfor betong |
| **Annet** | Waterstop/injeksjonsslange, fugeblikk, terreng, tekst – holdes utenfor betong |

Ukjente veggtyper vises som egen gruppe «Ukjent vegg: …», andre ukjente objekter under Annet → Ukjent.

## Mengder
- Volum = modellens volum (tykkelsene i modellen er riktige).
- Mangler volum men har areal: areal × tykkelse fra typenavnet (f.eks. Gulv på grunn 120mm).

## Funksjoner
- **Vis bare betongkonstruksjoner** (bryter): skjuler stål og annet. Av = alt vises igjen.
- **Grupper etter: Konstruksjon / PK** (PK = egenskapen «Pk Kode» fra Trimble Connect).
- Per gruppe: **Velg**, **Isoler**, **CSV**. Liste per type med flervalg (Ctrl/Shift).
- **Valgt i modellen**: m³, m², antall + CSV.
- **Stamp label**: «type · m³» per valgt element (maks 150).
- Hurtigminne: modell og GUID lagres per modellversjon; **Oppdater PK** henter nyeste PK, **Les modellen på nytt** leser alt.
- Støpestatus (farger) vises automatisk når modellen får «Støpe Dato».

## Data
All behandling skjer i nettleseren via Trimble Connect Workspace API og Trimble Connect sin Property Set-tjeneste (med din innlogging). Ingen data sendes til andre servere.

## Versjoner
- v0.1.0 – første versjon (basert på TB Betong Jåtunparken v0.4.0).
