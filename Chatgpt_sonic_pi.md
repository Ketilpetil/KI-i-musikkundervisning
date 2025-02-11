```
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
```
  with_fx :lpf, cutoff: 120 do
    sleep 8
    # Du kan legge til kode her for å justere cutoff dynamisk
  end
end
