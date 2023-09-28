+++
title = 'Ditt jobb är inte att koda'
slug = 'ditt-jobb-är-inte-att-koda'
image = '/images/posts/post-1/cover.jpg'
description = 'Det kommer en period i alla programmerares liv, där de inser att allt inte nödvändigtvis går att lösa med lite nästlade for-loopar'
disableComments = true
date = "2023-09-28"
+++

Och då tänker du förstås, **otur**, att koda var ju lite varför jag hamnade i den här branschen till att börja med. För att inte tala om, **va!?**, det står ju till och med ordagrant i mitt anställningskontrakt!?

*(Eller så är min bild av var utvecklare står i sin egen utveckling sned, och reaktionen är mer i linje med "no shit, sherlock"...?)*

Grejen är hursomhelst den att det är inte våra intrikata switch-satser eller inverterade röd-svarta-träd som någon betalar oss för. Det är för effekten vi har tänkt att de skall uppnå för någon användare i slutändan. Och även om vi *oftast* löser det med kod (det är ju just för att vi kan det som vi har jobbet) så är det mycket värt att först se problemen med rätt glasögon, eller från rätt vinkel om du vill. Då tenderar blir besluten vi tar något bättre något oftare. 

## Vi tar ett exempel

> En produktägare på en bank funderar över om det är en bra investering att utveckla en funktion för att kunderna ska kunna skjuta upp "sista betalnings-datumet" på fakturan mot en liten kostnad. A nominal fee. Vill kunderna ha det? Hur stor skall kostnaden i så fall vara? Kommer funktionen faktiskt få någon att hosta upp plånboken i praktiken?
>

> Är det lösbart med kod? Definitivt. Men går det att lösa på något billigare och snabbare sätt? Hur skulle det bli ifall vi fulhackade in alternativet direkt i frontend med lite A/B-testning för olika priser, men helt enkelt skita i att bygga funktionaliteten i backend? Förlänga fakturadatumet för kunden ändå och skicka något sött litet mail till kunden om att vi bjuder på avgiften.
> 

> Efter en vecka eller så tar vi bort fulhacket igen och har bra data att utgå ifrån för att mäta värdet av featuren. Visar datan att ingen ville ha det - så slapp vi en större utvecklingskostnad och kan lägga tiden och komplexiteten på något annat. Visar datan däremot att kunderna tyckte det var det bästa sedan skivat bröd och gladeligen kastar kronor på det - då vet vi bättre hur featuren skall prioriteras mot andra alternativ.
> 

## För kod är dyrt

Kod ruttnar, kräver underhåll, drift och övervakning. Och samordning. Till råga på allt gör det systemet mer komplext och mer svårutvecklat framåt. 

Sånt vill vi ju inte ha, usch för kod. 

Eller ptja, om vi slipper kod så är det ju inte helt dumt i alla fall.

Är det därför vi utvecklare har vår enorma trädgård med halvfärdiga open source-projekt som vissnar på GitHub? Vi kan koda precis vad lusten faller på och när det, lika överraskande varje gång, blir komplext och tråkigt så bara överger vi det.. efter vi släppt det som ett npm-paket förstås som någon stackare blir beroende av nästkommande 10 år.
<div style="display: flex; justify-content: center; flex-wrap: wrap;">
    <div>
        <a href="https://xkcd.com/2347/" target="_blank" > <img src="https://imgs.xkcd.com/comics/dependency.png" alt="XKCD explains"/></a>
    </div>
    <div style="flex-basis: 100%;  height: 0;"></div>
    <div style="font-size:small;"><a href="https://xkcd.com/2347/" target="_blank">[XKCD tells it like it is]</a></div>
</div>


<br/>
  
För att parafrasera Uncle Bob (från Clean coder vill jag minnas) så är en programmerares jobb att öka intäkter och minska kostnader genom automatisering. Torrt och trist, och inte i närheten ens av vad som fick oss att börja koda från första början. Jag vill lägga till “skapa nya möjligheter som inte fanns förut” på listan - men i slutet av dagen kan väl även det projiceras på någon av skalorna av intäkter och kostnader..

Deprimerad än? 🙂

Som tur är så kommer jobbet nästan alltid i praktiken handla om kod. Och när vi kommer från rätt vinkel så är det troligare att de lösningar vi gör inte behöver göras om, eller orsaka att vi behöver fulhacka ihop lösningar på nästa feature som skall byggas (eller leda till att det inte finns tillräckligt med intäkter för att betala din lön). Kodkvalitet och systemarkitektur är fortfarande viktigt - de är dock bara ett medel för att uppfylla det övergripande målet och inte ett egenvärde i sig själva. När vi talar om det ur den vinkeln så är dessutom risken att vi får lite mer gehör för vad vi vill säga större.

Som extra bonus behöver vi ju inte oroa oss över att AI kommer ta våra jobb - jobbet har ju aldrig handlat om själva programmeringen i vilket fall. Men det är ett ämne för en annan post.
