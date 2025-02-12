# KI på Musikklinja
# GÅ TIL https://urlr.me/qZaKXu
---
<table style="border: 1px solid #ccc; border-collapse: collapse; width:100%;">
  <tr>
    <td style="padding: 10px; background-color: white;">
      <strong> Jessheim VGS, 12.02.2025  <br><br>
Rom 3541 <br><br>
1430 - 1455 <br>
1500 - 1525<br>
1530  - 1555<br><br>


Internett:<br><br>
viken-gjest med gjestebruker 23657740<br>
passord: 6875
 </strong>
      <hr>
      <strong>Tema:</strong> Erfaringer med KI i musikklinjefag.<br><br>
      <strong>Eksperimenter underveis:</strong> Klikk på lenkene og følg oppskriftene.<br><br>


  </tr>
</table>


## Om meg

**Ketil Vestrum Einarsen**  
- Musikpedagog, underviser ved musikklinja på Jessheim MDD  
- Halvstudert "røver" i KI med videreutdanning i programmering og KI  
- Teknologioptimist, men kritisk til "Big Data"
- Bruker KI mye, fra å skape egen musikk til å effektivisere arbeidet på jobb

---

## Erfaringer med KI på musikklinja

### Begrepsavklaringer

- **KI-tjenester jeg snakker om i dag**
  - **Generativ språkbasert KI**  
    *Eksempel:* ChatGPT, Gemini, Perplexity osv
  - **Audio-/signalbasert KI**  
    *Eksempler:*  
    - Stemseparasjon (f.eks. [Spleeter](https://spleeter.online), eller integrert i Logic Pro og FL Studio)  
    - "Tekst til ferdige låter"-tjenester (f.eks. [Suno](https://suno.com))

[Plandagsangen](https://suno.com/song/75a3bc65-c218-4b9c-9a40-02bf6fa83258)




---

## Elevenes bruk av KI i i mine fag[^1]

- **Generativ språkbasert KI:**  
  - De aller fleste bruker gratisversjonen av ChatGPT.  
  - Enkelte benytter også NDLAs løsning.

- **KI i praktiske fag på musikklinja:**  
  - Bruken er generelt lav sammenliknet med andre fag. Men KI brukes i forskjellige former: 
    - **Stemseparasjon:** Elevene lager egne versjoner, for eksempel uten vokal, til øving eller fremføring. Noen elever bruker også dette til sampling. 
    - **Tekstskriving med ChatGPT:** Spesielt i komposisjonsoppgaver når tiden er knapp.



[^1]: Egne anekdotiske observasjoner med musikkelever på Musikklinja ved Jessheim. 


---

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
## LilyPond

Kort om LilyPond: Tekstverktøy for notasjon i tekstformat. Chatbotene kan eksportere og importere i lilypond. Elevene kan selv konvertere tekst til noter. 
Eksempel:
``` "Vis meg noter for en Fiss-dorisk skala i LilyPond-format. Jeg vil ha selve koden jeg kan lime inn i [hacklily](https://www.hacklily.org)```

Hvordan det fungerer:
- ChatGPT genererer koden.
- Elevene limer koden inn i en online editor (f.eks. hacklily).
- Dette testes sammen med noen interesserte elever. Test gjerne ut selv og kom med tilbakemeldinger. 
- Jeg har nettopp begynt å teste ut dette med NDLAs praterobot. Last opp [denne fila](https://github.com/Ketilpetil/KI-i-musikkundervisning/blob/main/Visning%20av%20noter-ndla-praterobot.json) [her](https://ndla-ki.no/prateroboter/apne-oppsett/). 

## Musescore

Kort om Musescore:
- Brukes til å skrive noter.
- Tidligere kunne ChatGPT lese og eksportere formater direkte fra Musescore.
- Nå (per 11.02): ChatGPT støtter ikke direkte import/eksport fra Musescore.
- Mulig løsning: Eksportere/importere formater (f.eks. MusicXML), men dette er tungvint og tidkrevende for elevene. [oppskrift ligger her](
](https://github.com/Ketilpetil/KI-i-musikkundervisning/blob/main/musicXML_til_chatbot.md)
## ChatGPT og programmering i musikkfaget

Styrke:
- ChatGPT er bra på programmering – også innen musikkprogrammeringsspråk som Sonic Pi.
- Eksempel: Genererte kodesnutter i Sonic Pi. Selv om låtene ikke alltid er fantastiske, gir de innsikt i prosessen og rom for læring og kvalitetskontroll.

Svakheter: 
- Vanskelig å finne plass til å gjøre dette på grunn av fagtrengsel og hva som står i kompetansemålene. 

https://github.com/user-attachments/assets/21f8a2d5-97cb-4dc8-aba9-f87400dafc73


- [Koden finner du her](https://github.com/Ketilpetil/KI_i_musikkundervisning/blob/main/Chatgpt_sonic_pi.md)


Kommentar:
- Jeg mener at Norge har ikke satset nok på programmering som tverrfaglig aktivitet. Matematikk "eier" faget i prasksis. Noe som fører til fagtrengsel i matematikk og at elevene går glipp av viktig læring. 
- En tverrfaglig implementering av programmering vil styrke både musikkfaget og elevenes digitale ferdigheter.


## Veien videre

- **Integrerte KI-løsninger:**  
  Læremidler i musikkfaget bør inneholde KI-verktøy som hjelper elevene med å utforske musikkteori, lydanalyse og skapende prosesser. Eksempler kan være:
  - Automatisert generering av noter.
  - Interaktive lydanalyser.
  - Dialog/feedback i skapende arbeid.
- Tjenestene må være gratis og tilgjengelige for alle.
- Tjenestene må forstå aktuelle filformater (som midi osv)

- Vi trenger verktøy som gir innsyn i kilder og metoder. 


- **Vi er de som vet hva vi trenger. Utviklerne trenger denne informasjonen** 

## S&S
- Har dere noen spørsmål?
- Har dere erfaringer dere vil dele?

## BONUS

Hvis vi rekker hører på vi to forskjellige eksempler med KI brukt i ny musikk. Hvis vi ikke rekker kan du sjekke det ut [her](https://open.spotify.com/playlist/1oUu9jpR4ShLU1cc2ExF9t?si=f0dafe742e6d4791) 





