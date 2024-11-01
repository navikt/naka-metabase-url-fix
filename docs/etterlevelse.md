---
title: Etterlevelse
---

## Hva er produktet?
"Etterlevelse" / "Støtte til etterlevelse" gir støtte til arbeidet med generelle regelverkskrav som gjelder for bredt for virksomhetens produkter, kalt [etterlevelseskrav](https://data.nav.no/begrep/BEGREP-1873). Løsningen støtter teamene som jobber med produktutvikling i å forstå og dokumentere etterlevelse av disse kravene. 

Kravinnholdet under et tema, forvaltes av de som har ansvaret for lovtolkning i organisasjonen (aka. "kraveier" eller "regelverkseier"). Kraveierne får gjennom løsningen støtte til å redigere og publisere etterlevelseskrav.

Etterlevelsekrav, etterlevelsesdokumentasjon og statistikk på dokumentert etterlevelse gjøres så åpent tilgjengelig som mulig. 


### Hva brukes produktet til?
Produktet adresserer:
* hvilke tema for krav som finnes
* hvilke regelverk som ligger under et tema
* hvem som har ansvar for tolking av regelverk
* hvilke krav og suksesskriterier som finnes for et regelverk
* hvilke spørsmål som er stilt til kraveier på et krav og hvilke svar som er gitt
* hvordan team dokumenterer sin etterlevelse
  * eksport av dokumentert etterlevelse til Word
  * arkivering av dokumentert etterlevelse til Websak

### Lenker
* [Om etterlevelsekrav i systemutvikling på Navet](https://navno.sharepoint.com/sites/intranett-utvikling/SitePages/Etterlevelseskrav.aspx)
* [Etterlevelse (prod)](https://etterlevelse.ansatt.nav.no/)
* [Etterlevelse (test)](https://etterlevelse.ansatt.dev.nav.no/)
* ["Om" seksjonen i selve løsningen](https://etterlevelse.ansatt.nav.no/help)

### Kontaktinformasjon
[Team Datajegerne](https://teamkatalog.nav.no/team/264cebfa-ad46-4af9-8867-592f99f491e6) utvikler og forvalter løsningen. Du kan nå teamet på slack [#etterlevelse](https://nav-it.slack.com/archives/C01V697SSR2)

### Administratorfunksjoner
* Administrasjon av tilgang til applikasjonen for kraveier og administrator.
* Administrering av kodelister, for å sikre datakvalitet er en rekke felter i løsningen basert på internt kontrollerte kodeverk. 
* Versjonshistorikk som inkludert timestamp , hvem som har endret noe, samt et snapshot av hele dataobjektet når det ble endret.

### Kildekode
* [Repo](https://github.com/navikt/etterlevelse)

### API
* [Swagger API](https://etterlevelse-api.intern.nav.no/swagger-ui/index.html)
* [Swagger API (Test)](https://etterlevelse-api.dev.intern.nav.no/swagger-ui/index.html)

### Datasett
* [Etterlevelseskrav i Metabase](https://metabase.ansatt.nav.no/browse/95-teamdatajegerne-etterlevelse-krav)
* [Etterlevelsesdokumentasjon i Metabase](https://metabase.ansatt.nav.no/browse/96-teamdatajegerne-etterlevelse-etterlevelse)

### Tilgang og headers
API er åpent for lesing for alle Nav-ansatte på en Nav-innrullert enhet, men eksponeres ikke eksternt utenfor Nav. 
Enkelte funksjoner er begrenset med rollestyring. Kontakt på #etterlevelse for mer info.

Headers
* Authorization - Systemer kan sende med Azure access token som Bearer token
* Nav-Call-Id - optional callId/correlation id to set for log tracing
* Nav-Consumer-Id - optional but strongly suggested to trace source of requests
