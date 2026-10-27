# DSGN Action Plans

Dashboard over handlingsplanerne i Buildings Design East (DSGN) i NIRAS CVI.

- Åbn siden og træk CSV-eksporten af SharePoint-listen med handlingsplanerne ind, eller vælg den med knappen »Upload ny CSV«.
- Filen læses kun i browseren. Intet sendes til GitHub eller andre steder.
- Den seneste fil huskes i din egen browser, så siden åbner med data næste gang. »Fjern data fra browseren« sletter kopien.
- Siden har ingen eksterne afhængigheder og virker også bag firewallen. Skrifttyperne er Aptos og Aptos Serif, hvis de findes på computeren.

## Hvad siden viser

- Nøgletal: antal handlinger, gennemsnitlig fremdrift, færdige, ikke påbegyndt og forsinkede.
- Fremdrift pr. strategisk spor (ringe), status pr. afdeling og en matrix over afdeling og spor.
- En tabel med søgning, sortering og filter på status. Klik på en handling for beskrivelse, ønsket resultat, statuslog og arbejdsgruppe.
- Forsinket betyder, at deadline-kvartalet er passeret, og handlingen ikke står til 100 %. »Ongoing« tæller aldrig som forsinket.

## Rapport som PDF

- Klik på »Lav rapport«. Rapporten følger dashboardets filtre (afdeling, spor, status og søgning) og tabellens sortering, så du filtrerer først og printer bagefter.
- Vælg titel, indhold (overblik, handlinger og detaljer), gruppering efter afdeling eller spor og papirretning.
- Detaljerne (beskrivelse, ønsket resultat, statuslog og arbejdsgruppe) står samlet i handlingens egen række. På liggende A4 står de som kolonner, på stående A4 lige under handlingen.
- »Vis rapport« viser A4-siderne. »Gem som PDF« åbner browserens udskriftsvindue, hvor du vælger »Gem som PDF«.
- Rapporten har hvid baggrund og kun små farvemarkeringer for at spare blæk. Tal og grafer beregnes på de handlinger, der er med.

## Filformat

CSV med komma, semikolon eller tabulator som skilletegn. Første række er kolonnenavnene fra SharePoint-eksporten. Påkrævet: `Department`, `Strategic track`, `Action name`, `Completion`. Brugt hvis de findes: `Description`, `Result`, `Status log`, `Responsible`, `Working group`, `Deadline [quarter]` (fx `2026Q2` eller `Ongoing`) og `Link to plan`.

Læg aldrig CSV-filer eller andre filer med tal i dette repo. Det er offentligt.
