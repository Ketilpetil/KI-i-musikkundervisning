# KI på Musikklinja

---

>Foredrag på Jessheim VGS, 12. februar 2025
Dere er velkomne til å teste ut alt jeg demonstrerer underveis – klikk på lenkene og følg oppskriftene.
Siden vi kun har 25 minutter, har jeg valgt å fokusere på noen få ting. 

## Om meg

**Ketil Vestrum Einarsen**  
- Musikpedagog, underviser ved musikklinja på Jessheim MDD  
- Halvstudert "røver" i KI med videreutdanning i programmering og KI  
- Teknologi- og musikkentusiast med interesse for å videreutvikle undervisningen  
- Teknologioptimist, men kritisk til "Big Data"  

---

## Erfaringer med KI på musikklinja

### Begrepsavklaringer

- **Deep Learning** (Goodfellow et al., 2016) danner grunnlaget for mange KI-tjenester.
- Vi kan dele KI i to hovedkategorier:
  - **Del 1 – Generativ språkbasert KI**  
    *Eksempel:* ChatGPT, Gemini, Perplexity osv
  - **Del 2 – Audio-/signalbasert KI**  
    *Eksempler:*  
    - Stemseparasjon (f.eks. Spleeter, integrert i Logic Pro og FL Studio)  
    - "Tekst til ferdige låter"-tjenester (f.eks. Suno)

---

## Elevenes bruk av KI

- **Generativ språkbasert KI:**  
  - De fleste bruker ChatGPT (ofte gratisversjonen).  
  - Enkelte benytter også NDLAs løsning.

- **KI i praktiske fag:**  
  - Bruken er generelt lav, men enkelte elever eksperimenterer med:
    - **Stemseparasjon:** Fjerner vokal fra spor for å bruke originalmusikk til øving eller fremføring.  
      *NB:* Finnes også som funksjon i programmer som Logic og FL Studio.
    - **Tekstskriving med ChatGPT:** Spesielt i komposisjonsoppgaver når tiden er knapp.

---

## Erfaringer fra undervisningen

### Bestefars julesangbot

- **Konsept:** Elevene skulle lage en "julesang for boomers" med hjelp av en ChatGPT-basert bot.
- **Fremgangsmåte:**  
  - Elevene skrev inn kilder, kompetansemål og atferdsregler.  
  - ChatGPT ga råd om sanginnhold, målgruppe og relevant musikkteori.
- **Resultat:** Vellykket, men begrenset av tjenestetilgang (bare betalende brukere har full funksjonalitet).  
  - Løsningen: Elevene måtte låne min datamaskin for å stille spørsmål – noe som ikke er en langsiktig løsning.

---

## ChatGPT og grafisk fremstilling av musikk

### ASCII-noter

- **Bruksområde:** Praktisk for å vise hvordan en skala eller akkord ser ut med enkle ASCII-symboler.
- **Utfordring:** ChatGPT (spesielt gratisversjonen) kan generere feil. Dette ble i praksis ubrukelig i undervisning. 
- **Læringsutbytte:** Elevene fikk se begrensningene til ChatGPT. 


#### Eksempel (kodeblokk):

```plaintext
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
```
## LilyPond

Kort om LilyPond: Et kraftig verktøy for notasjon i tekstformat.

Eksempel:
> "Vis meg noter for en Fiss-dorisk skala i LilyPond-format. Jeg vil ha selve koden jeg kan lime inn i [hacklily](https://www.hacklily.org)."

Hvordan det fungerer:
- ChatGPT genererer koden.
- Elevene limer koden inn i en online editor (f.eks. hacklily).
- Dette testes sammen med noen interesserte elever – responsen er lovende!

## Musescore

Kort om Musescore:
- Brukes til å skrive noter.
- Tidligere kunne ChatGPT lese og eksportere formater direkte fra Musescore.
- Nå (per 11.02): ChatGPT støtter ikke direkte eksport fra Musescore.
- Mulig løsning: Eksportere/importere formater (f.eks. MusicXML), men dette er tungvint og tidkrevende for elevene.

## ChatGPT og programmering i musikkfaget

Styrke:
- ChatGPT er svært dyktig på programmering – også innen musikkprogrammeringsspråk som Sonic Pi.
- Eksempel: Genererte kodesnutter i Sonic Pi. Selv om låtene ikke alltid er fantastiske, gir de innsikt i prosessen og rom for læring og kvalitetskontroll.

Kommentar:
- Norge har ikke satset nok på tverrfaglig programmering i musikkfaget, da andre fag (som matematikk) har fått mest fokus.
- En bedre forståelse av programmering vil styrke både musikkfaget og elevenes digitale ferdigheter.
- [Les mer om Sonic Pi-eksempelet her](https://github.com/Ketilpetil/KI_i_musikkundervisning/blob/main/Chatgpt_sonic_pi.md)


## Veien videre

- **Integrerte KI-løsninger:**  
  Læremidler bør inneholde KI-verktøy som hjelper elevene med å utforske musikkteori, lydanalyse og skapende prosesser. Eksempler kan være:
  - Automatisert generering av noter.
  - Interaktive lydanalyser.
  - Dynamisk feedback under komposisjonsprosesser.





Spørsmål til dere:
- Har dere noen spørsmål?
- Har dere erfaringer dere vil dele?
