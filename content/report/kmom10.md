---
Title: Kmom02
Description: Report for Kmom02
Template: kmom
---

 Report for KMOM10
==========================

Krav 1 Webbplats

Jag väljer en artist som min kund. Jag baserar innehållet på en kvinna jag känner.

Jag kopierar min portfolio och rensar innehållet helt förutom grundstrukturen. Jag tycker att det blir rörigt att hålla koll på exakt allt vad man har gjort i tidigare projekt och det uppstår konflikter mellan nytt och gammals kod. Jag finner det enklare att bygga upp från grunden och låna bitar av min kod efter behov än att förändra saker i existerande kod. Innehållet är rätt enkelt. Jag uppdaterar package.json för ett nytt tema och justerar twig-filen för att använda -min versionen av css-filen. Jag skapar .md mallar för hem-, om- och kontaktsidorna, och en mapp för highlights vilket är överdrivet eftersom det blir inga följdsidor (jag tänkte göra separata sidor för varje exempel men insåg att det inte behövdes). Jag kontrollerar att alla sidor laddar rätt innehåll och att länkar funkar.

Krav 2

Jag designar sidan i Adobe XD. Jag ville prova verktyget som nämndes i början av kursen - det går snabbt att lära mig och jag har hela designen framför mig. Jag placerar relevanta bilder för varje sida i meta-informationen och hämtar de i twig när det behövs. Jag kämpar lite med placeringen av bakgrunden och löser det med hjälp av background-position: 50% 0%.
Jag testar att basera min layout på 'grid layout' med 9 kolumner, men inser att layouten är egentligen inte så komplicerat och lämnar idén, i stället lägger jag grid när det behövs in containern och använder procentantal för att justera kolumnbredden (på tex about-sidan).
Jag skriver om färgval, design och sass strukturen [här](http://www.student.bth.se/~ankv20/dbwebb-kurser/design/me/kmom10/aboutsite).
Det är mkt enklare att skriva temat med hela designen färdig. Dock iom att designen skiljer sig någorlunda på varje sida gör jag versioner av .container elementet som .about-container och .highlights-container.
När jag skriver texten om sidan (den dolda länken [här](http://www.student.bth.se/~ankv20/dbwebb-kurser/design/me/kmom10/aboutsite)) använder jag cimage i markdown. Annars använder jag det direkt i twig-filerna.

Krav 3 Responsivitet och tillgänglighet

Jag skapar separat scss fil för responsivitet och lägger till den på slutet av min style.scss. I devtools hoppar jag mellan olika mobilskärmstorlekar för att säkerställa att mina justeringar funkar för alla.
Jag använder viewport width för textstorleken på loggan och vissa marginaler. Jag använder background-position för att bakgrundsbilden ska vara på rätt plats för hemsidan och alla grids som en kolumn.

Tillgänglighet-checken gör att jag ändrar all min textfärg förutom på hemsidan till en mörkblå färg som jag sätter som svart i variablerna och minskar opaciteten på bakgrunden. Jag tycker det blir mindre elegant än vit text, men kontrasten är högre.

Colorblind Web Page Filter visar ett bra resultat och jag gör inga ändringar.

Krav 5 Analys aktuell webbplatsdesign

Jag väljer att analysera 5 sidor för advokatfirmor i London som jag ursprungligen undersökt för projektet (jag tänkte först göra en just sådan sida). Det finns många likheter och en del olikheter så att det blir lite mer varierande analys. Jag tittar igenom ett urval av undersidor först och får ett generellt intryck. 5 sidor ger mer data att gå på än 3 som jag gjorde i uppgiften för portfolion. Jag dokumenterar sen färgval, logotyp, typografi samt generella designbeslut och jämför dem i slutsatsen. En bra övning för att titta med mer distans på sidor, vad som funkar och inte och lära sig.

Allmänt
Jag tyckte projektet var relativt lätt att genomföra och definitivt är ett rimligt projekt för denna kurs. Dock spenderar jag lite längre tid än önskat. Dock lär jag mig att prioritera dock och jag är mer nöjd med min tidsåtgång än i förra projektet. Jag är särskild nöjd med att ha testat XD och designa helheten först. Att ha en helhetsbild i tanken genom hela processen hjälper otroligt mycket, samt att ha en referens man kan gå tillbaka till. För en riktig sida skulle jag spendera mer tid på att identifiera gemensamma faktorer såsom marginaler och padding för text tex, så att de behöver inte justeras för enskilda element. I många fall handlar justeringar ändå om slarviga värden som kanske inte behövs (tex padding höger OCH vänster om bara vänster behövs).

Jag väljer att gör bakgrund med hjälp av clip-path och det blir huvudvärk eftersom jag lyckas inte få den formen att vara lika hög som innehållet. Min footer hamnar utanför. Jag flyter footern ovan i stället, men relativa värden i höjden på vissa element gör att layouten går sönder i alla fall. Frågor jag har är: ska man försöka anpassa design för många skärmstorlekar eller låta bli och fokusera på de vanligaste (ser inte de flesta på sidorna i fullskärm storlek iaf?)? Är det värt att överväga noggrannare vilka värden är relativa och vilka är fasta? Kanske kommer med erfarenhet.

Jag väljer också göra bakgrund-grafiken med inverterade färger på olika sidor och fixar det med olika css taggar (.colour-background och .white-background).

Om Kursen

Jag tycker om ämnet sen tidigare - grafisk design och estetik är mina favoriter. Jag är rimligt nöjd med kursen. Jag anser att Pico är ett bra grund för att fokusera på css och design. Kanske pga mina tidigare kunskaper själv skulle jag vilja dyka in lite djupare och kanske få mer feedback på själva design-delen. Jag känner att jag gör uppgifterna och får tummen upp, dock ingen feedback som skulle hjälpa mig utvecklas. Samtidigt förstår jag att kanske ambitionsnivån för just design-delen är inte så hög för just det här programmet.
Jag tycker om att arbeta med Niklas. Han ger sakliga svar snabbt och håller god stämning överlag. Emils föreläsningar hade jag svårt för. Jag tyckte de var onödigt detaljerade, eller kanske långsamma och på det viset ofokuserade. Jag hade svårt att känna mig engagerad trots mitt intresse för ämnet. Jag har ingen tvekan om att Emil har mycket att bidra med kunskapsmässigt men presentationen står i vägen för det. Förövrigt hade jag inget problem med språket (jag nämner det för att han bad om ursäkt för brytningen).
Jag skulle nog kunna rekommendera den här kursen till någon som är nybörjare i webbdesign. Kursen får 7/10 av mig.  
