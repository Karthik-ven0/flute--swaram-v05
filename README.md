# Bansuri Guru v0.5 — maker chart + live swara detection

## New in v0.5
- Replaces the earlier generic Sa illustration with the six-hole fingering chart transcribed from the Radhe guide image you provided.
- Includes Sa, Re, Ga, Ma, Pa, Dha, Ni and the higher Sa row.
- Live detected shuddha swara highlights its corresponding fingering row.
- Live swara tiles still follow the detected note automatically, including naming komal/tivra variants.
- For komal/tivra notes not shown in the supplied chart, the app explains that it has no fingering from this chart rather than guessing.
- Fixes a stray escape sequence in the earlier script, ensuring JavaScript globals are separated by a real newline.
- Keeps the microphone workflow and local audio processing.

## Run
Do not open index.html directly; microphone use requires HTTPS or localhost.
1. Extract this ZIP.
2. Run `python -m http.server 8000` inside the folder.
3. Open `http://localhost:8000` in Chrome.
On Android, deploy to an HTTPS host and open that URL in Chrome, then allow microphone access.

## Important limitations
This is an early prototype. The pitch detector can confuse harmonics, noise, and weak fundamentals. Microphone pitch detection can't confirm actual finger coverage. The chart patterns transcribe the supplied manufacturer image, and advanced/komal/tivra fingerings should be confirmed from the course/manual.
