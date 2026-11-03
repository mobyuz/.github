# Moby

**A voice-enabled AI companion robot for your Windows PC.**

Moby Mini is a compact ESP32-S3 robot with an animated OLED face. We're building it so you can press a button, speak a request, and have Moby carry out tasks you approve on your PC. For example, you could ask it to check the Git status of a project you select.

<p align="center">
  <img src="https://raw.githubusercontent.com/mobyuz/3d-model/main/moby-mini-assembled.png" alt="3D render of Moby Mini showing the OLED eyes, microphone mute switch, and Talk button." width="480">
  <br>
  <em>Blender render of the Moby Mini enclosure</em>
</p>

## How Moby is designed to work

1. **Robot.** Press the Talk button to start voice capture. The OLED shows when Moby is listening, muted, or disconnected. A physical mute switch disconnects the microphone's data line.
2. **Windows app.** The robot connects to your PC over USB. The app keeps conversation history on your PC and checks permissions before carrying out local actions.
3. **Moby API.** With your consent, the app sends voice requests to the server. The API handles speech transcription, AI replies, and speech synthesis.

## Repositories

| Repository | What's inside |
| --- | --- |
| [moby-firmware](https://github.com/mobyuz/moby-firmware) | C firmware built with ESP-IDF, including OLED expressions, button and mute-switch handling, and a microphone bench test. |
| [moby-api](https://github.com/mobyuz/moby-api) | Rust, Axum, and PostgreSQL API for accounts, sessions, consent, and usage limits. Includes an OpenAPI contract and mock AI and voice responses. |
| [moby-web](https://github.com/mobyuz/moby-web) | Project website built with React, TypeScript, and Vite. |
| [3d-model](https://github.com/mobyuz/3d-model) | Blender models, parts list, and wiring for Moby Mini. |

## Project status

Moby is in the prototype stage. The firmware builds and has passed automated tests. The next steps are testing the microphone and controls on a physical board and connecting the robot, Windows app, and API for end-to-end voice requests. You can run the API locally with Docker Compose and the website with Vite. See each repository for setup instructions.
