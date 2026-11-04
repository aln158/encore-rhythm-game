# Source-matched holds — frozen v2 asset revision

Song: `encore-original-metal-v2-holds`. Chart: `encore-original-sparse-v2-holds`. This is the project's original procedural composition; no commercial recording or imitation was introduced.

All 256 original required onset IDs, roles, keys and times are unchanged. 24 existing heads now use actual sustained notes: bass 8 × .75 seconds, rhythm 8 × .9 seconds, lead 8 × 1.2 seconds. The other 232 heads remain taps; all 64 drum heads remain taps. The first bass hold starts at 7.5 seconds so the opening notes teach taps first.

44 non-required accompaniment onsets were suppressed to avoid interruptions of the same held instrument. The audio waveform, source ledger and chart were regenerated together. Main WAV hashes changed; intro-ending.wav is unchanged.

`hold_evidence.json` records source ID, start/end, instrument, technique, source sustain, sample range, current stem hash and final-150ms signal energy. Every held note has no other same-role source onset inside it and no required note through the extra 120ms release allowance.

Runtime contract: tap/hold onset gives one immediate attack; maintained hold is visual/sustain feedback only; successful completion may give one finite bonus/charge; never award every frame. Early release loses completion reward only and preserves the original valid onset. Hold heads are excluded from optional demolition offers.

Validation: five chart/waveform tests pass; actual Chrome decoding verifies four equal 120-second stems, a clipping-free combined peak of 0.8800012 and a sample-identical repeated first second after looping. Human listening approval is not claimed.
