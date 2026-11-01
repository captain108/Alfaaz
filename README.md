# Alfaaz screen-accurate visual recreation

This project recreates the *visible website content inside the laptop display* from the supplied 54-second reference recording.

## What is included
- 809 perspective-corrected screen frames sampled at 15 FPS from the original 30 FPS recording.
- The original recording's audio extracted to MP3.
- A custom HTML Canvas player that renders the screen-frame sequence in sync with the extracted audio.
- Play/pause, seek, restart, volume, mute and fullscreen controls.

## Run on Zorin OS
1. Extract this ZIP.
2. Open the `alfaaz-screen-recreation` folder.
3. Double-click `index.html` and open it in Chrome or Firefox.
4. Press Play. Fullscreen gives the best result.

No Node.js, Java, server, npm packages or internet connection are required.

## Important technical note
The source recording does not contain the original website's HTML/CSS/JS or separate source assets. This is therefore a high-fidelity screen reconstruction using the extracted display frames as an image sequence, not the original site's editable source code. The sequence excludes the laptop body and the camera surroundings. The frame sequence runs at 15 FPS (half of the source 30 FPS) to keep the package and playback load manageable.
