# KI i musikkundervisning

Velkommen! Dette dokumentet presenterer erfaringer og eksempler fra bruk av KI i musikkundervisning. Under foredraget deler jeg skjerm med GitHub (Markdown) og inviterer dere til å lese direkte på deres maskiner.

---

## Om meg

**Ketil Vestrum Einarsen**  
- Musikpedagog, underviser ved musikklinja på Jessheim MDD  
- Halvstudert "røver" i KI med videreutdanning i programmering og KI  
- Teknologi- og musikkentusiast med interesse for å videreutvikle undervisningen  
- Teknologioptimist, men kritisk til "Big Data"  
- Bruker mac på dagjobb og Linux ellers

---

## Erfaringer med KI på musikklinja

### Begrepsavklaringer

- **Deep Learning** (Goodfellow et al., 2016) danner grunnlaget for mange KI-tjenester.
- Vi kan dele KI i to hovedkategorier:
  - **Del 1 – Generativ språkbasert KI**  
    *Eksempel:* ChatGPT
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
- **Utfordring:** ChatGPT (spesielt gratisversjonen) kan generere feil – men feilen blir en læringsmulighet.

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
