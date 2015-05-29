---
title: AlltidBuss Infoskjerm
---

En ny versjon av Android-appen AlltidBuss Infoskjerm er ute! Last den ned [her](https://play.google.com/store/apps/details?id=no.vtek.alltidbuss "Google Play").

## Litt historie

AlltidBuss Infoskjerm er en app som inneholder en widget man kan plassere på hjemskjermen på telefonen. Denne widgeten fungerer som en klone av de skjermene som henger rundt om i busskur i Trondheim og omegn. Man kan ha flere widgeter samtidig, og innholdet oppdateres ved en tap.

Da jeg begynte med denne appen gikk jeg fortsatt på skolen. Jeg hadde nettopp hatt, eller var midt oppi, et Android-fag, og var mildt sagt veldig fascinert av denne utviklingsplatformen. Tenk så kult det ville være å ha sin egen app på telefonen!

### Ville ta i bruk nylært kunnskap

Jeg vet ikke hva som kom først; ønsket om å lage en app, eller interessen for å utforske APIet til AtB. Det ble i hvert fall til at jeg fikk kobinert de to interesseområdene og laget min første app.

### Arbeide med data fra den "virkelige verden"

Det tok noe tid før jeg fikk tildelt en API-nøkkel (som kreves for å bruke APIet), men når den kom var det bare å teste ut mulighetene. Jeg husker jeg slet ei god stund før jeg skjønte hvordan APIet fungerte, da jeg var fremmet for både SOAP-protokollen og italiensk, som API-et snakker. Ja, det stemmer – italiensk. Etter god hjelp av Google Translate og et online SOAP-testeverktøy fikk jeg dog hentet ut det jeg trengte for å presentere interessant informasjon i min egen løsning.

### Første versjon

Appen ble først publisert i 2012, og har egentlig fungert vedlikeholdsfritt. Det har hent at den ikke får opp informasjon, men da har det vært pga. trøbbel hos AtB, så det har holdt å vente litt. En gang var det dog litt værre. De bestemte seg plutselig for å skifte datoformat, og da sluttet alt å fungerte. Heldigvis oppdaget jeg feilen kjapt og fikk rettet opp det. Ikke særlig bra fra AtBs sin side å gjøre sånne endringer uten å sende ut en mail til de med API-nøkkel, om jeg får lov til å løfte en pekefinger.

### På tide med en oppussing

Jeg gikk lenge og tenkte på å lage en ny versjon av appen. Det var noe funksjonalitet jeg savnet, og så tenkte jeg at det hadde vært kult å lage noe til iPhone i tillegg.

Det ble gjort noen forsøk, og jeg gikk litt fram og tilbake, men til slutt fant jeg ut at jeg ville bygge videre på den funksjonaliteten som allerede var der, uten å endre så mye på brukergrensesnittet.

Kodebasen til den originale appen var mildt sagt utdatert, både med tanke på Android APIet og mine ferdigheter, så jeg bestemte meg kjapt for å starte fra scratch. Jeg tok utgangspunkt i utseende til den gamle appen, og fikk gjenbrukt noen grafiske elementer, men stort sett ble strukturen bygd helt annerledes for å være både "penere" og mer robust.

### Nye behov og ønsker

Funksjonelt sett savnet jeg mest muligheten for å filtrere avganger på rutenummer, slik at jeg kun fikk se de avgangene jeg var interessert i. På bussholdeplasser der mange forskjellige ruter passerer (Solsiden f.eks.), var det ikke uvanlig at min buss ikke engang kom opp i lista, som begrenset seg til de 5 neste avgangene. Dette var neste utvidelse jeg ønsket – mulighet for flere enn 5 avganger.

Jeg jobbet noen kvelder, og fikk en tilfeldig interessert til å være prøvekanin, og ikke lenge etter fikk jeg endelig publisert en ny versjon – to og et halvt år etter forrige. Følgende liste ble "changelog" til den nye versjonen:

* Mulighet for å filtrere hvilke bussruter som vises
* Mulighet for å vise flere avganger (opptil 30)
* Høyden på widgeten kan justeres
* Widgeten kan legges på lock screen der det er støttet

Jeg håper jeg med denne oppdateringen gjorde appen enda bedre for dere som liker å bruke den, samtidig som den kanskje ble mer interessant for de som ennå ikke har prøvd den.

Spre gjerne ordet. Jeg begynner å nærme meg 1000 brukere, men det er et lite stykke igjen.