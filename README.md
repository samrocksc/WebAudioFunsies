# Testing out web audio live recordings

base-intervals - []()https://flashy-approval.surge.sh/

## General Notes About The WebAPI

- WebAudio records agt 44.1khz(aka 441000/second);
- AnalyserNode will provide you with an array of 1024 numbers.
- Wavelength is _technically_ measured on a wavelength's crest to crest; however...for the sake of pitch bending/vibrato it's saner to measure where the node thresholds are crossed.
- AnalyserNode returns a length y height of `0-256` meaning that the node for the sound wave is `128`.
