# KI i musikkundervisning

## Om meg: 

Ketil Vestrum Einarsen
musikpedagog. underviser i fag på musikklinja på Jessheim MDD. 
Er halvstudert røver i KI, med videreutdanning i programmering og i KI. 
Men jeg er Teknologi og musikk-teknologientusiast og er interessert i hvordan vi kan videreutvikle undervisning med ny teknologi. 
Nokså teknologioptimistisk, men kritisk til "Big Data". Bruker mac på dagjobb og Linux ellers. 

## Erfaringer med KI på musikklinja.


Begrepsavklaringer: 


Deep Learning av Goodfellow et al. (2016): 

Del 1 – Generativ språkbasert KI
Eksempel: ChatGPT

Del 2 – Audio- eller signalbasert KI
Eksempel: Stem-separasjon med Spleeter, integrert i Logic pro og FL studio. 
brukes til re-mastering, karaoke, sampling mm. 
I tillegg, "tekst til ferdige låter"-tjenester som Suno. 



Elevenes bruk av KI på musikklinja

Nesten alle som bruker Generativ språkbasert KI bruker chatGPT. De aller fleste har gratisversjonen.  Noen bruker NDLAs løsning. 


Elevene på alle trinn bruker Generativ språkbasert KI nokså lite i praktiske fag. Det finnes noen unntak: 
Et unntak er at noen elever bruker stem separation. Bruken av dette ser ut til å øke. 
Stem separation deler låta opp i separate filer. Et praktisk eksempel på dette er elever som fjerner vokalen fra et spor for å bruke orginalmusikken til øving eller fremføring. 
(Et online eksempel? pluss nevne mest brukte tjenester, og kanskje si at dette finnes i programmer som logic og FL studio?)

Et annet unntak er at de bruker chatGPT til å skrive tekster. Gjerne i en kontekst der de ikke har tid til å fokusere på tekst, som i oppgaver med komposisjon. 

Siden ChatGPT kom har jeg prøvd ut hvordan forskjellige KI-tjenester kan brukes i praktisk undervisning på musikklinja. Jeg har tenkt å dele erfaringene og komme med en statusrapport på hvor vi er. Jeg skal prøve å være veldig rask, slik at det blir tid til innspill fra dere. 

Utgangspunktet mitt for dette har vært å utforske om det finnes måter elever kan brukes ChatGPT og andre tjenester på en konstruktiv måte i skapende aktiviteter i musikkundervisning på VGS. Personlig føler jeg elevene trenger mer trening og forståelse i anvendt musikkteori. Jeg har lett etter måter ChatGPT kan vise informasjonen de trenger på en bra måte, gi dem god informasjon, og ikke minst - gå i dialog med elevene. 

Var det en suksess? Svaret er sammensett, men kort fortalt: Elevenes tilgang begrenser kvaliteten på tjenesten.  

Har vi fått noe bra ut av det? 
Ja. Både i forhold til elevenes kompetanse i musikk, og i forhold til digitale ferdigheter og i forhold til å utvikle kritisk tenkning. 




Eksempler på hva vi har gjort i undervisningen: 


Bestefars julesangbot:


ChatGPT gir oss muligheten til å dele "boter" vi selv lager. Man kan svært enkelt legge inn ting som kilder, kompetansemål og beskjeder om atferd. Elevene mine hadde fått i oppgave å skrive en "julesang for boomers". De kunne spørre chatboten om råd, og den kom med råd om innhold i sangen, informasjon om målgruppa og aktuell musikkteori. 
Dette fungerte veldig bra. 

Problemet er bare at dette er en tjeneste som er tilgjengelig for de som betaler for tjenesten. Eleven endte opp med å låne min datamaskin for å stille spørsmål. Dette er selvsagt ikke en løsning som vi kan leve med. 


# ChatGPT og grafisk fremstilling av musikk

Kort tekst her om hvorfor dette kan være nyttig....

1.  ASCII-symboler. "Lenke til fila her" 


Jeg fant ut av ChatGPT faktisk kan "tegne" noter eller annen informasjon med ASCII. Dette kan være praktisk for elever som lurer på et konkret spørsmål, hvordan en skala ser ut, for eksempel. 

Men, den er, tilsynelatende ikke trent i dette. Og det dukket opp veldig mye feil. Særlig gjaldt dette gratisversjonene elevene brukte. Men også i betalingsversjonen oppdaget jeg feil. 
h
ttps://github.com/Ketilpetil/KI_i_musikkundervisning/blob/main/chatbotprompter.md


Her er et eksemep: 

(Må stå som kodeblokk i markdown)

                (Treble Clef Staff)
      ┌─────────────────────────────────┐
(Line 5)  F ─────────────────────────────
(Line 4)  D ─────────────────────────────
(Line 3)  B ────────────●───────────────   (● markerer G)
(Line 2)  G ─────────────────────────────
(Line 1)  E ────────────●───────────────   (● markerer E)
      └─────────────────────────────────┘

Ekstralinje (Ledger line) under notestaven:
           ───── ● ─────  
                  ^
                  C  (Middle C)


Men, ChatGPT tilsynelatende ikke trent i dette. Og det dukket opp veldig mye feil. Særlig gjaldt dette gratisversjonene elevene brukte. Men også i betalingsversjonen oppdaget jeg feil. Det som riktignok var en suksess her, var at elevene selv kunne se problemene og begrsnisningene til ChatGPT. 


2. Noter i tekstformat: 




## Lilypond:

Kort om lilypond her. 
ChatGPT kan skrive noter


Vis meg "Skriv inn det du trenger her"  LilyPond-format. Jeg vil ha selve koden jeg kan lime inn i [hacklilly](https://www.hacklily.org)
Elevene limer inn et prompt og stiller et spørsmål til chatGPT. Deretter limer de inn teksten de får tilbake på en nettside. 
Dette tsster  jeg nå sammen med noen interesserte elever. Det ser lovende ut, jeg har testet dette noen runder og fått riktige svar. Dersom dere ikke gjør det, ta kontakt med meg. 

## Musescore

Kort om musescore. Dersom elevene mine kunne hatt meningsfulle diskusjoner med ChatGPT om det de skriver i dette programmet, tror jeg de kunne utviklet seg. Tidligere kunne ChatGPT lese og eksporter formater som man kunne eksportere fra Musescore. Dette kan chatGPT , per 11.02 ikke gjøre. 
Men, det er mulig å eksportere/importere formater som chatGPT leser. Jeg har testet ut dette. Det fungerer bra, men løsningen er tungvint. Mange elever synes det er vanskelig å sette opp detsom skal til, og dette vil stjele fra undervisningstiden. 

3. Er det noe ChatGPT er veldig god på i musikkfaget? 

Programmering. Her er et eksempel på noe som CchatGPT genererte til musikkprogrammeringsprsåket Sonic Pi. Det er riktignok ikke en fantastisk låt. Men den gir oss noe som Suno ikke gjør, vi ser det so skjer mellom tekstprompt fra ChatGPT og lyden treffer ørene våre. Da kan vi som lærere kvalitetssikre det og elevene kan lære av det. 

Den er trent på mye tekstm inkludering programmeringsspråk. Norge, i motsetning til mange andre land, har ikke satset på å gjøre programmering til et tverrfaglig disiplin. Det er matte som har fått jobben. Det er riktignok en del av kompetansemålene i musikk på ungdomsskolen. Og det kan absolutt forsvares å jobbe med ut i fra kompetansemål på musikklinja. Men, fagtrengsel setter effektivt en stopper for det. 
Personlig skulle jeg sett at vi klarte få plass til dette i musikk. Grunnen til at jeg tenker det er at det er et problem med tjenester som suno. Vi vet ikke hva som skjer "mellom teksten som skrives og den ferdige låta". Jeg tror elevene våre lærer veldig lite av dette. De får ikke se prosessen, vi i får ikke innsyn i prosessen. Hverken metoder eller kilder er noe vi får tilgang på. 
Men, jeg tror elevene våre kan lære mye av musikk og samtidig forstå og mestre KI-tjenster dersom de hadde lært seg programmering bedre. 


(Technolåt)[https://github.com/Ketilpetil/KI_i_musikkundervisning/blob/main/Chatgpt_sonic_pi.md]

avskutningsvis lurer jeg på to ting: 

har dere noen spørsmål?
har dere noen erfaringe dere vil dele? 




