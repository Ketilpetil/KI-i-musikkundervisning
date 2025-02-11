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



Bestefars julesangbot:


ChatGPT gir oss muligheten til å dele "boter" vi selv lager. Man kan svært enkelt legge inn ting som kilder, kompetansemål og beskjeder om atferd. Elevene mine hadde fått i oppgave å skrive en "julesang for boomers". De kunne spørre chatboten om råd, og den kom med råd om innhold i sangen, informasjon om målgruppa og aktuell musikkteori. 
Dette fungerte veldig bra. 

Problemet er bare at dette er en tjeneste som er tilgjengelig for de som betaler for tjenesten. Eleven endte opp med å låne min datamaskin for å stille spørsmål. Dette er selvsagt ikke en løsning som vi kan leve med. 

ASCII-symboler. "Lenke til fila her" 

Jeg fant ut av ChatGPT faktisk kan "tegne" noter eller annen informasjon med ASCII. Men, den er, tilsynelatende ikke trent i dette. Og det dukket opp veldig mye feil. Særlig gjaldt dette gratisversjonene elevene brukte. Men også i betalingsversjonen oppdatet jeg feil. 


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





# Welcome to Sonic Pi

###############################################################################
# Techno-inspirert låt i Sonic Pi
# Forfatter: ChatGPT
# Basert på ideer fra Sam Aarons metode med live-koding
###############################################################################

use_bpm 125  # Sett tempo/bpm for låten

#######################
# 1. Grunnleggende KICK
#######################
live_loop :kick do
  sample :bd_tek, amp: 2  # Bruk en techno-aktig bassdrum
  sleep 1  # 1 slag per kvart
end

################################
# 2. Hi-hat og perkusjon (off-beat)
################################
live_loop :hihat do
  sync :kick  # Synkroniser start med kick
  sample :drum_cymbal_closed, amp: 1, rate: 1.5
  sleep 0.5  # Spiller hver 8. del
end

################################
# 3. Sub-bass (Synth)
################################
live_loop :bass do
  sync :kick
  use_synth :tb303  # Typisk syre/techno-synth
  use_random_seed 2023  # For litt varierende basslinje
  8.times do
    play :e1, cutoff: rrand(70, 100), res: 0.9, release: 0.3, amp: 0.8
    sleep 0.5
  end
end

################################
# 4. Acid-lignende melodi
################################
live_loop :acid_melody do
  sync :kick
  use_synth :tb303
  use_random_seed 1234  # Endre tall for å få nytt mønster
  16.times do
    note = (scale :e2, :minor_pentatonic).choose
    play note, release: 0.125, cutoff: rrand(70, 110), res: 0.9, amp: 0.6
    sleep 0.25
  end
end

################################
# 5. Tekstur og effekter (Pad)
################################
live_loop :pad do
  sync :kick
  use_synth :prophet
  with_fx :reverb, room: 0.8, mix: 0.5 do
    play_chord chord(:e4, :minor), release: 4, cutoff: 80, amp: 0.3
    sleep 8
  end
end

################################
# 6. Ekstra perk (klapp eller snare)
################################
live_loop :clap do
  sync :kick
  sleep 1  # Venter 1 takt før vi spiller klapp
  sample :perc_snap2, amp: 1.5
  sleep 1
end

################################
# 7. Master FX
################################
# Et eksempel på hvordan du kan styre lydbildet
live_loop :master_fx do
  with_fx :lpf, cutoff: 120 do
    sleep 8
    # Du kan legge til kode her for å justere cutoff dynamisk
  end
end

