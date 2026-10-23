# DSGN KPI Dashboard

Kvartalsdashboard for Buildings Design East (DSGN) i NIRAS CVI. Afløser `index.html` (v1.4.0) i roden af repoet.

- Åbn siden og træk KPI-filen (CSV, semikolon-separeret, fx `KPIs_to_track11.csv`) ind, eller vælg den med knappen.
- Filen læses kun i browseren. Intet sendes til GitHub eller andre steder, og intet gemmes, når fanen lukkes.
- d3 v7.9.0 er bygget ind i `index.html`, så siden ikke henter kode udefra. Kun skrifttypen hentes fra Google Fonts, hvis Aptos ikke findes på computeren.

## Hvad siden viser

- Seks nøgletal for det valgte Til-kvartal mod samme kvartal året før: omsætning og EBITA år til dato, SU, FTE, personaleomsætning og sygefravær.
- Faner: Økonomi, Udnyttelse (SU), Projektmix, Medarbejdere, Størrelse, Diversitet og uddannelse samt Alle tal.
- Margin beregnes af EBITA ÷ omsætning. Kvartalets egne tal beregnes som år til dato minus kvartalet før.
- Kvartaler med 0 i HC og omsætning regnes som ikke indrapporteret og vises ikke.

## Filformat

Første række: to tomme felter og derefter kvartaler som `2024Q1;2024Q2;…`. Hver række: `ID;Navn;værdi;værdi;…` med dansk decimalkomma og evt. `%`. Rækkerne genkendes på navnet (fx `Total revenue`, `ASIC, SU`, `PLED, FTE`). Nye afdelinger med `XXXX, SU` eller `XXXX, FTE` kommer automatisk med. Rækker siden ikke kender, nævnes øverst på siden.

Læg aldrig KPI-filer eller andre filer med tal i dette repo. Det er offentligt.
