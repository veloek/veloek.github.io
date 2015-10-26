---
title: Trondheim Developer Conference 2015
---

TDC 2015 er nå historie, og jeg sitter igjen med mye ny kunnskap og innsikt i noe av det som beveger seg i utviklermiljøet. Nye og spennende prosjekt er på vei inn i varmen, og mange har lagd mye kult med eksisterende teknologi. Jeg oppsummerer det jeg fikk med meg på konferansen.

Det har vært en fullspekket dag, med foredrag som har tatt for seg alt fra fascinerende canvas-animasjon i JavaScript, til hacking av avanserte våpen for å få full tilgang til det underliggende Linux-baserte operativsystemet.

Det var flere foredrag jeg ikke fikk med meg, da de overlappet andre enda mer spennende titler, men sånn vil det vel alltid være når det er så mye bra innhold som skal porsjoneres ut over et relativt kort tidsrom. Forhåpentligvis vil opptakene (for jeg tror alt ble tatt opp) bli lagt ut, så det blir mulig å se det man gikk glipp av.

Jeg vil i denne oppsummeringen ta for meg noe av innholdet i de foredragene jeg fikk med meg. Det er sikkert mye jeg glemmer å skrive om, men jeg skriver det jeg husker.

### Keynote

Etter registrering og den første kaffekoppen var det duket for konferansens keynote. Jeg visste ikke hva jeg skulle forvente, men TDC traff blink her. Talen ble holdt av Seb Lee-Delisle, en britisk karakter som hadde like lett for å snakke for en stor forsamling som for å kode. Han viste eksempler på prosjekter han har jobbet på, og det var den ene fantastiske oppvisningen etter den andre. Her snakker vi store scener og mye fancy utstyr (type lasere og led-montasjer) på enorme lerret, gjerne påvirket av publikums bevegelser eller tilhørende musikk.

Seb Lee-Delisle hadde en karisma i retning av Graham Norton og fikk en veldig god tone med publikum. Han demonstrerte underholdene eksempler av canvas-animasjon i JavaScript, der han tegnet opp et tre som beveget seg i vinden, bygd opp av en rekursiv funksjon med noe hjelp av Math.random. Ikke mange linjer kode her altså, og alt ble skrevet på scenen. Han beskrev seg selv som en "artsy" person som lager kunst med kode, eller evt. en programmerer som lager "artsy" ting.

Keynoten gav en flott start på programmet, og gjorde at jeg gledet meg enda mer til å høre de andre foredragene. Seb Lee-Delisle var nok kanskje den beste taleren, og det at han i tillegg til å være "artsy" og flink til å snakke, er en stor nerd og god til å kode, var veldig imponerende.

### The Extensible Web, Houdini and CSS.next

Bruce Lawson tok for seg webstandarder og hvordan det fungerer når flere aktører som lager nettlesere går sammen for å bli enige om ny funksjonalitet. Det tar tid. Og av og til blir det lagd funksjonalitet som ikke stemmer helt overens med behovet hos webutviklere, som for eksempel webcache.

Han tok opp en del nye ting vi kan glede oss til, som bedre støtte for å "offline" webapps, der vi kan bruke service workers til å snakke med nettleseren, selv når enheten ikke er tilkoblet Internett. Det skal bli lettere å få webapps til homescreen, i stedet for å måtte åpne nettleseren og navigere i bookmarks for å finne appen.

Mye av foredraget handlet om å ta bort mye av magien bak det som skjer i nettleseren, og la webutviklere "tappe in" på det som skjer i bakgrunnen. Jeg synes det høres ut som en god ide og gleder meg til å se mulighetene som kommer.

### Beyond REST/JSON: Cross-platform APIs with Thrift and Protobuf

Fra Zedge kom CTO Stig Bakken for å snakke om alternativer til REST/JSON API, med hjelp av Thrift eller Protobuf. Dette var ny teknologi for meg, men det var spennende å høre om andre måter å ta for seg kommunikasjon på. Thrift og Protobuf er to prosjekt som tar for seg samme problem, men så vidt jeg forstår har Thrift støtte for flere språk. Thrift er fra Apache, mens Protobuf er fra Google.

Målet er å ha en felles måte å serialisere data og sende det fram og tilbake mellom forskjellige system av ulike programmeringsspråk, slik at det blir lettere å snakke sammen. Man skriver en spesifikasjon av hva som skal utveksles, og så kan man generere kode for forskjellige språk. Deretter kan man implementere funksjonaliteten, og så vil Thrift eller Protobuf ta seg av selve kommunikasjonen.

Dette er definitivt teknologi jeg vil utforske nærmere dersom jeg kommer over et prosjekt der jeg må kommunisere mellom forskjellige komponenter skrevet i forskjellige språk. Inntil videre føler jeg det er enklest å lage små REST-baserte API og bruke den gode støtten for AJAX-forespørsler som finnes i de store, kjente JavaScript-rammeverkene.

### Enkel RESTFull tjeneste med .NET, Vagrant og Docker

Andreas Mosti fra DIPS skulle demonstrere en setup der han bruker Vagrant og Docker, men på grunn av problemer med tilkoblingen til projektoren, ble det litt amputert. Han fikk likevel beskrevet mulighetene med disse verktøyene på en god måte.

Jeg har selv så vidt begynt å bruke Vagrant, og jeg ser virkelig verdien i å kunne scripte et utviklingsmiljø som så kan settes opp i Windows, Linux eller OS X ved å kjøre én kommando; vagrant up. Dette gjør at man slipper å tenke på forskjellige versjoner av serverprogramvare, manuelt oppsett av virtuelle maskiner, eller konfigurering av WAMP, LAMP, etc. Docker har jeg ikke prøvd ennå, men jeg har fått med meg at det har tatt av og blitt veldig mainstream. Jeg forstår det slik at det letter deployment-biten ved at man har alle dependencies samlet i en "pakke" som kan kjøres uavhengig av andre biblioteker og systemer.

Andreas Mosti snakket også om Mono-prosjektet, og hvordan det har tatt av etter Xamarin tok over og ble store på cross platform-utvikling av mobil-apps. Mono er dog også bra på andre platformer, og nå har det blitt tatt inn i varmen av Microsoft, som tidligere var litt skeptisk til prosjektet. Jeg kommer ikke på hvilket verktøy Andreas nevnte, men han snakket om self-hosting ASP.NET-applikasjoner som kjører på Mono, og det er jo veldig interessant når man slipper å kjøre IIS for å hoste applikasjonen.

### Lunch

Etter lunchen var det kun ett foredrag på programmet; Lunch av tegneserieskaper Børge Lund. Dette foredraget handlet lite om programvareutvikling, men var likevel veldig underholdende. Børge kunne fortelle at han har en mastergrad i industriell design. Og med en bakgrunn fra forskjellige kontorjobber, hadde han et godt grunnlag for å skape god humor i striper som treffer godt ting vi kan kjenne igjen fra vår egen hverdag.

Gjennom å vise hvordan han jobber når han bygger opp en ny stripe, fikk vi litt innsikt i hva man må tenke på når man skal lage en tegneserie. Han viste også noen teknikker for å tegne karakterer, og hvordan man ved å endre noen få linjer linjer, kan gjøre stor forskjell i ansiktsuttrykk og formidling.

Jeg har ikke lest så mye Lunch, men jeg kommer til å gjøre det mer etter å ha hørt fordraget til Børge Lund.

### When IoT attacks: Hacking a Linux-powered rifle

Når jeg ser hacking, Linux og rifle i en og samme tittel, er dette nok til å fange min interesse. I dette foredraget fortalte Runa A. Sandvik om hvordan hun og ektemannen sammen tok ei "smart-rifle" og fikk tilgang til det underliggende operativsystemet.

Rifla de hadde jobbet med var ei TrackingPoint TP750. Dette er ei rifle med et såkalt smart-scope. Det vil si at det er en liten datamaskin i kikkertsiktet som hjelper skytteren med å treffe målet sitt. Det fungerer slik at man setter et merke på målet sitt, og så vil ikke rifla avfyre skuddet før den vet at den treffer målet.

Runa og ektemannen så på appen som følger med og fant ut av noen av tjenestene rifla tilbyr over HTTP. Dette var dog ikke nok til å få full tilgang til funksjonaliteten, så de skrudde den fra hverandre og fikk dumpet innholdet i en brikke på kretskortet som inneholdt filsystemet. Derifra kunne de lage seg en falsk programvareoppdatering de kunne pushe til rifla som lot de få root-tilgang til operativsystemet. Med denne tilgangen kunne de gjøre alt de ville, og de hadde tilgang til å korruptere parametre til programvaren, slik at en skytter kunne bruke rifla i god tro, men bomme på målet den hadde satt. Den svakheten de tok utnyttelse av er dog kun mulig dersom rifla er satt opp til å kommunisere med appen over wifi.

### React Native

Det har i mange år vært snakk om webapps og hybride mobilapplikasjoner, skrevet i HTML og JavaScript, som et enklere alternativ til å skrive native kode for hver platform.

Emil Mork snakket litt om utfordringene med dagens hybridapplikasjoner og hvorfor han tror React Native er en bedre tilnærming. React Native fungerer slik at man skriver en JavaScript-applikasjon, og så vil UI-et rendres natively, mens logikken foregår i en JavaScript-motor i en annen tråd. På denne måten vil brukergrensesnittet være like kjapt som i en native-applikasjon, mens man kan debugge og live-oppdatere JavaScript-koden fra Chrome på utviklingsmaskinen. Han gikk ikke så mye inn på detaljene rundt kodingen, men det hørtes ut som man kan dele veldig mye av kodebasen for Android og iOS. Det var dessuten ikke så vanskelig å utvide funksjonaliteten med egne "plugins" for å få tilgang til forskjellige native API.

Jeg tror i likhet med Emil Mork at dette er en god måte å angripe problemet på, og det er fint med et friskt pust på et område som stort sett har basert seg på Cordova og WebView. React og React Native kommer fra Facebook, og det virker som de satser stort på dette. Det at det kommer fra Facebook, gjør at det får stor omtale og mange utviklere tar det i bruk. Det er dog veldig ferskt ennå og det har noen sterke konkurrenter, så det blir spennende å se hvordan det klarer seg framover.

Et annet alternativ til React Native er NativeScript, men det ble ikke et tema i dette foredraget. Det er dog verd å sjekke ut.

### Intro to ASP.NET 5 - Open Source and Cross Platform

Microsoft har våknet og oppdaget at det er smart å inkludere flere platformer og miljøer i teknologien sin. Derfor har de åpnet kildekoden til flere prosjekt, deriblant ASP.NET og .NET Core, og satset på å lage kode som fungerer cross platform. Dette gjør at det blir enklere å bygge .NET-applikasjoner for Linux og OS X. I tillegg støtter de Linux-miljø i cloud-tjenesten sin Azure.

Scott Hanselman jobber med open source hos Microsoft og snakker om spennende ting som skjer der. Med ASP.NET 5 blir det lett å bygge f.eks. en webapplikasjon i C# og kjøre det på en Linux-server. Dette demonstrerer han på en tilfeldig Macbook og en Raspberry PI. Han demonstrerer også fin funksjonalitet i Visual Studio Code via OmniSharp som gir Intellisense til C#-prosjekter. OmniSharp støtter dog også mange andre editorer, som Sublime Text, Emacs og Vim.

Alt i presentasjonen er fint og flott, men det hele minner litt om Java. Se her, vi kjører på alle platformer med samme kompilerte kildekode. Det er likevel kult at Microsoft satser på mer åpenhet og viser bedre samarbeidsvilje med open source-miljøet.

### Writing cross platform mobile apps with Cordova

Sahli Malik tok for seg Cordova, og da i sammenheng med Ionic Framework. Ionic utvider Cordova på kommandolinja og bygger på AngularJS i rammeverket sitt. De har mange fine grafiske komponenter som gjør det enkelt å komme i gang med en hybridapplikasjon hvis man er kjent med Angular.

Det mest spennende med foredraget var integrasjonen i Visual Studio og hvor enkelt man kan sette opp en byggserver i OS X. Uten veldig mye arbeid har man en tjeneste som kjører i OS X som man kan koble seg opp mot i Visual Studio, og med et slikt oppsett kan man bygge Cordova-applikasjoner for alle enheter rett fra Visual Studio. Fordelen med dette er at man får brukt den gode debuggeren som finnes i VS, i stedet for å måtte bruke Safari og debuggeren der i OS X.

### JavaScript, The Cloud, and the Rise of the New Virtual Machine

Helt til slutt var Scott Hanselman tilbake på scenene for å runde av konferansen. Det siste foredraget handlet om JavaScript og skyen, og hvordan ting har forandret seg siden tiden hvor man måtte ta seg av skalering ved å kjøpe inn og konfigurere hardware selv.

Scott snakket om hvordan JavaScript nesten er som en virtuell maskin inne i nettleseren, hvor det kan ta seg av mye av det samme som et operativsystem, det være seg rendring av et brukergrensesnitt, io-kommunikasjon over nettverket, minnehåndtering, osv.

Scott Hanselman var en av de beste foredragsholderene, og det var nok derfor han hadde 3 foredrag på TDC. Han var flink til å holde en lett og spøkefull tone, samtidig som det var interessant og lærerikt det han kom med. Han har vært med i gamet i mange år og viste at han har mye kunnskap på mange områder.

Som flere andre, spådde han at der noe kan skrives i JavaScript, kommer det til å bli skrevet i JavaScript. Jeg er redd han har rett, og derfor er jeg glad for at det stadig kommer nye verktøy og rammeverk som gjør hverdagen til webutviklere bedre.

Takk for en flott konferanse. Det var en fryd å være deltaker og jeg kommer gjerne igjen.