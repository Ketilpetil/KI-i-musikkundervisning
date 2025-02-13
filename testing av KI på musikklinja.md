# KI på Musikklinja
---
Siden oppdateres kontinuerlig. 

## Erfaringer fra undervisningen

### Bestefar Boomers Julesangmentor
![image](https://github.com/user-attachments/assets/056fbc00-1bd6-43a1-96c3-7466e7b5b8c6)

- **Konsept:** Elevene skulle lage en "julesang for boomers" med hjelp av en ChatGPT-basert bot. 
Gå til [GPTs](https://chatgpt.com/gpts) for å finne ut mer om hvordan du kan lage boter selv. 
- **Fremgangsmåte:**  
  - Jeg skrev skrev inn kilder, kompetansemål og atferdsregler.  
  - ChatGPT ga råd om sanginnhold, målgruppe og relevant musikkteori.
- **Resultat:** Vellykket, men begrenset av tjenestetilgang (bare betalende brukere har full funksjonalitet).  
  - Løsningen: Elevene måtte låne min datamaskin for å stille spørsmål – noe som ikke er en langsiktig løsning.


Kan ikke brukes på grunn av at tjenesten ikke er tilgjengelig. 

---

## ChatGPT og grafisk fremstilling av musikk

### ASCII-noter

- **Bruksområde:** Praktisk for å vise hvordan en skal eller akkord ser ut med enkle ASCII-symboler.
- **Fremgangsmåte:** Elevene limte inn tekstprompter til chatgpt for å få ChatGPT til å vise en grafisk fremstilling av noter. Du kan finne promptene [her]. 
- **Utfordring:** ChatGPT (spesielt gratisversjonen) svarte feil. Dette ble i praksis ubrukelig i undervisning. 
- **Læringsutbytte:** Elevene fikk se begrensningene til ChatGPT og de fikk muligens styrket digital kompetanse. 


#### Eksempel:

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

Kommentar 13.02.2025: Kan ikke brukes på grunn av kvaliteten på svarene til chatbotene

## LilyPond

Kort om LilyPond: Tekstverktøy for notasjon i tekstformat. Chatbotene kan eksportere og importere i lilypond. Elevene kan selv konvertere tekst til noter. 
Eksempel:
``` "Vis meg noter for en Fiss-dorisk skala i LilyPond-format. Jeg vil ha selve koden jeg kan lime inn i [hacklily](https://www.hacklily.org)```

Hvordan det fungerer:
- ChatGPT genererer koden.
- Elevene limer koden inn i en online editor (f.eks. hacklily).
- Dette testes sammen med noen interesserte elever. Test gjerne ut selv og kom med tilbakemeldinger. 
- Jeg har nettopp begynt å teste ut dette med NDLAs praterobot. Last opp [denne fila](https://github.com/Ketilpetil/KI-i-musikkundervisning/blob/main/Visning%20av%20noter-ndla-praterobot.json) [her](https://ndla-ki.no/prateroboter/apne-oppsett/). 

Kommentar 13.02.2025: Lovende, men noen problemer knyttet til versjoner av lilypond og syntax. Kan kanskje løses med beskjeder til chatbotene. 


## Musescore

Kort om Musescore:
- Brukes til å skrive noter.
- Tidligere kunne ChatGPT lese og eksportere formater direkte fra Musescore.
- Nå (per 11.02): ChatGPT støtter ikke direkte import/eksport fra Musescore.
- Mulig løsning: Eksportere/importere formater (f.eks. MusicXML), men dette er tungvint og tidkrevende for elevene. [oppskrift ligger her](https://github.com/Ketilpetil/KI-i-musikkundervisning/blob/main/musicXML_til_chatbot.md)

Kommentar 13.02.2025:
Fungerer bra, men begrensninger på antall tegn i gratistjenestene kan være en potensiell hindring. Elever skal teste. 
Tungvint løsning, leter etter en bedre løsning for å få ned antall steps. 


## ChatGPT og programmering i musikkfaget

Styrke:
- ChatGPT er bra på programmering – også innen musikkprogrammeringsspråk som Sonic Pi.
- Eksempel: Genererte kodesnutter i Sonic Pi. Selv om låtene ikke alltid er fantastiske, gir de innsikt i prosessen og rom for læring og kvalitetskontroll.

Svakheter: 
- Vanskelig å finne plass til å gjøre dette på grunn av fagtrengsel og hva som står i kompetansemålene. 

https://github.com/user-attachments/assets/21f8a2d5-97cb-4dc8-aba9-f87400dafc73


- [Koden finner du her](https://github.com/Ketilpetil/KI_i_musikkundervisning/blob/main/Chatgpt_sonic_pi.md)




