# Vision

## Bakgrund
Det är ett ständigt återkommande mantra för oss som verkar i skolan i allmänhet och på tekniska program i synnerhet att en majoritet av elever läser väldigt få böcker. Det är ett problem då läsning är grundläggande för en utvecklad språklig förmåga, och en mycket stark prediktor för möjligheten att klara av tertiär utbildning. I de fall där vi lyckats med att få elever att läsa regelbundet rapporterar de ofta ökat fokus, bättre sömn, och bättre framgång i såväl språkämnen som matematik och fysik. Det finns försök i skolor med att införa läsning varje morgon, eller till och med som inledning till varje lektion, och resultaten är oftast mycket positiva, och verkar vara ett mer effektivt sätt att främja arbetsro än det omdiskuterade mobilförbudet. 

På gymnasieskolan Stockholm Science & Innovation School (härefter förkortat SSIS), i Kista norr om Stockholm, jobbar vi på att lansera ett läsfrämjande program. En central del av detta program är en bokcirkel som planerats under en längre tid. I och med detta föddes också tanken om att ha en digital miljö kopplad till denna bokcirkel.

### Problembeskrivning
Att starta en bokcirkel är i sig ganska lätt, men att hålla igång en sådan är en större utmaning. Hur ska vi välja ut böcker? Hur ska vi få en levande diskussion som inte bara sker i organiserade möten, där det kan finnas en möjlighet att läsningen blir en aktivitet som fortgår utan att lärare är ständigt närvarande? 

En sida där eleverna kan logga in, skapa sina bokhyllor, rekommendera och diskutera böcker, leta efter inspiration, ställa frågor och skriva ner reflektioner skulle i bästa fall kunna vara ett verktyg för att stötta oss lärare i detta arbete, och bli ett forum för eleverna att utvecklas. 

## Målgrupp
Målgruppen är i första hand tänkt specifikt för eleverna på SSIS, det vill säga gymnasieelever som går på Teknikprogrammet och som har ett stort intresse för IT. Målgruppen kan gärna breddas till gymnasieelever i allmänhet, om detta skulle vilja tas upp av andra gymnasieskolor. En sekundär, men viktig, andra målgrupp är personalen på SSIS, både lärare och vår IT-tekniker som om projektet mynnar ut i en produkt vi vill använda kommer att ansvara för driften av den. 

## Marknad
Den första frågan som man kan ställa sig är förstås varför vi inte bara använder oss av Goodreads, som redan är den stora aktören vad gäller att lägga upp bokhyllor, recensera böcker, diskutera med mera? Det finns några problem med att som skola använda sig av en aktör som Goodreads, och det är att vi kanske vill använda oss av plattformen som en del av skolarbetet vid någon tidpunkt, och det är inte förenligt med GDPR och skollag att använda en sida som Goodreads för skolrelaterade interaktioner med elever. Det underlättar mycket att vi kan kontrollera vår egen data och hålla dem i våra egna nätverk och servrar. 

Ett annat alternativ vore att skapa ett utrymme i vår lärplattform (Instuctures Canvas) för detta ändamål, men dels så kan vi inte styra utformningen för att få all den funktionalitet som vi önskar (det blir exempelvis svårt att göra egna bokhyllor i Canvas). Det är också osäkert att kunna ha det beständigt i lärplattformen, då det inte är säkert att vi vill eller får fortsätta använda den.

En sista och mycket viktig aspekt av egenutvecklad vs Goodreads är att vi kan engagera eleverna i plattformens fortsatta utveckling, och styra funktionaliteten såsom vi vill att den ska vara - inklusive en integration med Goodreads via deras API. Då vi är en skola som profilerar sig med mycket egenutveckling och samarbeten, så ligger det mer i linje med våra övergripande tankar att ha vår egen sida med koden publikt vår vår egen gitlab. 

## Egenskaper
I SSIS bokcirkel så ska du som användare kunna ha sin egen bokhylla, där man kan lägga upp såväl lästa böcker som böcker man är intresserad av. För dessa böcker ska man kunna recensera, kommentera, reflektera, betygsätta för egen del, men också delta i diskussioner kring eller rekommendera böcker till en annan användare. 

## Teknik
SSIS bokcirkel byggs i node.js. 
- Ramverk: Vue?
- databas: MongoDB, Mongoose. 
- Ubuntu server. DigitalOcean eller direkt på skolans server?
- Bokinformation KB via deras API
- Tester: Mocha, Chai, Jest
- Tillgänglighetsanpassad. (http://wave.webaim.org/, CKEditor 4, www.boia.org?)
- Stretch Goal - integration med Goodreads?


I detta projekt för vi även in ett avsnitt kring tekniker du tänkt använda dig av, då detta är en viktig punkt i dessa projekt. Tekniker kan väljas utifrån tidigare erfarenhet, att man vill testa eller lära sig något, industristandard, tillgänglighet, etc. Teknik kan vara alltifrån val av programmeringsspråk, speciella api:er, ramverk, hårdvaruplattformar, servermjukvaror etc.


Mattias Wickberg, Webbprogrammerare