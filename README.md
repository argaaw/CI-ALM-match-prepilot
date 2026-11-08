# CI-ALM match pre-pilot (SSD-CI similarity survey)

Static survey page for an informal pre-pilot: Korean SSD-CI listeners rate how similar five cochlear-implant simulations
sound to the original heard through their implant (7 clips x 5 conditions, 7-point labelled scale: 1 very different … 7 very similar). Responses go to the existing
Supabase Edge Function (evaluation id `ssdci-match-prepilot-001`). Built by `scripts/prepilot_remote_build.py` in the
CI-ALM-difficulty repository; do not edit by hand.

## transcription/ — informal transcription pilot (2026-10-18)

Self-administered page for an informal pilot: SSD-CI listeners stream one sung lyric line at a time to the implant and type what they hear, with up to 5 plays per line (every attempt is saved). 15 items + 2 practice items + 1 setup test clip; evaluation id `ssdci-transcription-pilot-001` on the same Edge Function. `transcription/monitor.html` shows one participant's attempts live. Built by `scripts/pilot_transcription_build.py` in the CI-ALM-difficulty repository; do not edit by hand.

## nh/ — informal NH transcription pilot (2026-11-08)
Same 15 items, 2 practice items and setup clip as `transcription/`, played to normal-hearing lab colleagues over earphones as a cochlear implant simulation (me201_song or peters_a_noise). One link; the condition is assigned when a new participant code is entered, to the condition with fewer entrants so far (ledger rows under participant `nhassign-ledger`; codes starting with `test` are not counted, `test-a` / `test-b` force a condition). Evaluation id `nh-transcription-pilot-001`, participant id `nh-<code>`. `nh/monitor.html` shows one participant's attempts. Built by `scripts/pilot_transcription_build.py --listener nh` in the CI-ALM-difficulty repository; do not edit by hand.
