+++
title = 'Gillar du inte Scrum?'
slug = 'gillar-du-inte-scrum'
image = '/images/posts/post-2/kanban monkeys.jpg'
description = 'Då skulle ni sett vad vi hade innan… eller vad vi kommit på numera!'
disableComments = true
date = "2023-09-29"
+++

Vattenfallsprocessen, RUP eller varför inte Cowboy. Att vara utvecklare i början av 2000-talet (och tidigare), det var tider det. Vi byggde system som var oanvändarvänliga och inte riktigt löste det de skulle. Missade deadlines gjorde vi också, hela tiden, även fast det tog **år** att få ut saker genom dörren. Hittade på dumheter som “*code freeze*” och “*stabilization periods*”. Ja, jösses.

Inte undra på att några smarta filurer samlades runt en whiteboard 2001 och skrev ett [manifesto](https://agilemanifesto.org/) över hur vi skulle **sluta utveckla mjukvara på så dumpuckat sätt.** 

Lite samma drivkraft låg bakom att jag snöade in på agila metoder. Det började med den lilla goa boken [Scrum and XP from the trenches](https://www.crisp.se/bocker-och-produkter/scrum-and-xp-from-the-trenches) av [Henrik Kniberg](https://www.crisp.se/konsulter/henrik-kniberg) (kanske mest känd från Spotify) och hade väl sitt crescendo när jag gick Scrum master-certifieringen med just Henrik och en av grundarna av Scrum ([Jeff Sutherland](https://en.wikipedia.org/wiki/Jeff_Sutherland)). Var helt enkelt less på att ständigt vada i gegga, buggar och “all hands on deck”.

Lade enorma insatser på att få till användbara estimat och hålla sprintar. En dans, såhär i efterhand, med kanske en gnutta överskattat värde. 

Missförstå inte; för många (kanske de flesta?) utvecklarteam så är Scrum bra (kom ihåg vad vi hade innan). Hela poängen med Scrum är att visualisera vad tusan vi håller på med och framförallt att **få folk att prata med varandra**. Vi utvecklare är ju skitbra på att hitta på sätt så vi slipper just det - vi uppfann ju till och med *Pull requests* för att slippa att ha med andra människor att göra IRL. True story.

## Men det finns ju andra sätt än Scrum.

Det har nog inte gått någon förbi att det här med estimat funkar lite sisådär. Ordet på gatan är att det är ett NP-komplett problem. Det enda man vet om estimatet och om medföljande deadline är att det är precis då det inte kommer vara klart.

Men vi vill så gärna få den sköna känslan av kontroll och förutsägbarhet som vi får av att kunna peta in siffrorna i vårt excel-dokument - att vi forskat fram en hel del sätt att förbättra träffsäkerheten (planning poker etc). I slutet av dagen så är ändå användbarheten av estimat: sisådär. Det största problemet jag har med estimat är att de ger en skenbar bild av verkligheten som är helt oförankrad i just, verkligheten. 

Estimeringen har dock en väldigt stark fördel skall sägas - **det tvingar oss att prata ihop oss** innan vi kastar iväg en slev kod på ett problem. Men måste vi verkligen sitta med Jira burndown charts och en kortlek för att lyckas med det?

Tänk om vi kan lägga den tiden och insatsen på att faktiskt skapa något av värde[tm] istället. Våra slutanvändare skiter ändå i hur bra vi är på planning poker - de vill att vår slutprodukt löser ett problem åt **dem** i slutändan.

## **Jobba utan estimat, sprintar och påhittade deadlines**

> Jag tänker: MVPs, hur vi skriver stories, WIP-limits, parprogrammering, code reviews och standups.
> 

### 1. Minimum viable product

Steg ett är att bryta ner det vi vill åstadkomma till minsta möjliga release av minsta möjliga värde för slutanvändaren. Få ut något **framför ögonen på våra slutanvändare** så fort det bara går - för sen kommer vår förståelse för vad vi skall göra förbättrats (och förändrats - om vi byggt mer så hade det varit till stor del varit waste). Det är ett helt orimligt krav att någon skall veta vad de vill ha när det kommer till mjukvara - vi människor funkar helt enkelt inte så. Ut med något i händerna på användaren, lär av feedbacken och planera först då för nästa steg. 

### 2. User stories

För att realisera MVPn behöver vi ha en samstämmig bild av vad det är vi skall åstadkomma. Dags att börja bryta ner i några stories (eller vad vi vill kalla dem). Tumregeln för en story är att när den är klar, så skall den vara releasad och bidra med **något användbart för slutanvändaren**. Det innebär att vi inte delar upp arbetet beroende på teknikområde (frontend/backend/infrastruktur etc) utan på effekt vi vill åstadkomma med systemet (som bonus hjälper det oss med struktur för samarbete).  Den skall även vara så liten som möjligt, minimum viable story (MVS?) om du så vill. “Genomföra en betalning med kreditkort” istället för “Bygg formulär för att skriva in kreditkortsnummer” t.ex.

### 3. Kanban board

När vi har en tillräckligt stor (läs: liten) hög med stories att bygga, så är det dags att slänga upp dem på en Kanban board - som i en simpel form kan bestå av 5 steg/kolumner: 

- Att göra
- Under utveckling
- Test/QA
- Release
- Färdig

*(Jag vill gärna ha med två steg till; Cleanup och utvärdering, men det får bli ett ämne för en senare post).*

Det vi gör nu är att vi sätter en “work in progress”-begränsning (**WIP-limit**) på varje kolumn så att färre saker kan vara under utveckling än vad vi har medlemmar i teamet! Om vi är 4 utvecklare så får det vara max 3 stories i “under utvecklings”-kolumnen t.ex. Det är så vi med hjälp av struktur hjälper oss att prata med varandra och samarbeta. 

I praktiken betyder det att när vi är färdiga med något i exempelvis Test/QA, så får vi inte dra in något nytt från “*att göra*”-kolumnen, ifall “Under utveckling”-kolumnen redan är full. Då får vi först kolla hur vi kan hjälpa de som sitter på de befintliga lapparna med att få ut grejerna, tänk: parprogrammering. Eller ptja, egentligen först kolla om något ligger i release eller test/QA som skall vidare och jobba oss tillbaka mot “att göra-kolumnen”. (Exakt, även utvecklare kan testa av saker, det kommer lite med konceptet att samarbeta som ett team)

> Hela idén är att få folk att prata med varanda och samarbeta, samt att följa principen att **********************************det oftast är bättre att avsluta saker än att påbörja nya**********************************.
> 

### 4. Standup

Detta får vi pejl på under standup - en procedur som kan ha dåligt rykte på grund av hur meningslöst den ofta genomförs. Poängen med standup är att “**under dagens förutsättningar planera hur vi på bästa sätt uppnår våra *mål* just idag”** - (tänk: får ut skit i prod och utvärderar tänkt effekt/hypotes).

Det handlar **inte om vad du gjorde igår, vad du gör idag eller om du har några blockers**. Vårt jobb är inte att hålla oss sysselsatta - vårt jobb är att åstadkomma rätt effekt. 

Vi fokuserar på det arbete som är igång och hur vi på bästa sätt får färdigt och slutför det. Så vi börjar från höger på tavlan (”Release”) och frågar hur vi bäst organiserar oss för att få ut det som ligger där. Sen fortsätt vi åt vänster kolumn för kolumn, story för story, och till slut så kommer nog alla ha att göra ändå. Som bonus kommer vi dessutom veta allt relevant som gjordes igår eftersom det tas upp på respektive story av de som råkade sitta på den, och vi vet vad alla kommer göra idag och om några **storys** har blockers.

### 5. Code review

Nu när alla vet vad de håller på med (för de flesta, typ samma som igår) så jobbar vi på med planen för dagen för att få färdigt grejer. Och innan något är färdigutvecklat så är det dags för en code review. Dags att prata med varandra, igen!? (vi kan slippa om vi parprogrammerat, då är det fullt rimligt att anse att koden redan är reviewad) 

Poängen med code reviews är alltså framförallt att vi pratar med varandra om hur vi gör saker. Att vi följer en konsekvent tanke om hur vi vill ha det i vår kodbas. Sprider kunskap och synsätt. Minskar “bus factor”. **Jobbar tillsammans, lär av varandra**. Som bonus förekommer vi kanske lite buggar, hittar saknade testfall och liknande - men det är mest en bonus. 

Sättet att genomföra det med mest bang for the buck är i min bok “axel-mot-axel”-reviews. Vi tar helt enkelt och sätter oss framför samma skärm och går igenom och framförallt diskuterar igenom allt. Även det otränade ögat ser ju att detta går alldeles utmärkt att göra remote med lite skärmdelning - fast jag är tämligen övertygad om att vi vinner väldigt mycket mer på att göra det på plats.

### 6. SHIP IT!

När releasar vi till prod? Hela tiden. **Heeela tiden.** Continuous integration/Continuous deployment (CI/CD) är inte en diskussion längre (precis som enhetstester inte är), det är en hygienfaktor. Små releaser ger små risker och färre buggar. Det visste redan de gamla grekerna! Så vi sätter upp vår pipeline så att vi hela tiden kan skeppa det vi bygger utan att störa användarna av systemet. 

För att inte låta kod ligga och ruttna i feature branches för länge - använder vi **feature flags**. Poängen med Continuous integration är just själva ordet integration. Och continuous. Git flow är för boomers, vi försöker undvika feature branches in i det sista - och när det ändå är vettigt att använda sådana - merge:ar vi in dem i main så fort som möjligt.

### You build it, you own it

Sen var det ju det här med **DevOps** också. Finns lite olika definitioner på vad det innebär (lite som när företagen som körde vattenfallsprocessen i början av 2000-talet bytte ut ordet till Scrum i sina dokument och plötsligt var “agila”). I min värld innebär DevOps att teamet äger hela processen - från idé till utveckling, till deployment, drift och övervakning. **Inget är någon annans problem** helt enkelt. Vem kunde tro att det skulle göra susen för kvaliteten? Lite av det revolutionerande med hela moln-revolutionen(?) var att infrastruktur nu är såpass standardiserad och förenklad att det går att hålla koll på.

## Sist men inte minst

Så är en sån här process till för att hjälpa teamet, **inte styra teamet**. Det kommer uppstå tillfällen då det bästa är att göra undantag - och då gör vi så klart det. När det är ett sådant tillfälle lär vi oss av erfarenhet; någonstans mellan “*att göra så många undantag att vi inte har någon process kvar*” och “*att svära för ofta över att krångla till stegen med mer procedur och byråkrati än nödvändigt*”. Men vi har ju retrospectives för sådana reflektioner och diskussioner, inte sant?

Känns det väldigt annorlunda mot hur du jobbat hittills? Under många år i min karriär så funderade jag på om det var jag som var galen, eller *alla* andra. Läste söta bloggartiklar om testdriven utveckling, continuous delivery och andra vackra ord - men såg det aldrig i verkligheten. Känner du igen dig i det så vill jag bara trycka på att du är inte galen. Det finns där ute - sättet att jobba på i den här posten är helt baserat på verklig erfarenhet. Vi jobbade såhär under många år och med stor framgång (även om det självklart aldrig är problemfritt och utan komplikationer - det finns ingen silver bullet).