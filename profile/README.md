<h1 align="center">Moby</h1>

<p align="center"><strong>A voice-enabled desk robot for Windows.</strong></p>

<p align="center">
  <img src="https://raw.githubusercontent.com/mobyuz/3d-model/main/moby-mini-assembled.png" alt="Moby Mini showing its OLED eyes, mute switch, and Talk button." width="420">
  <br>
  <em>Moby Mini · Blender render</em>
</p>

Moby Mini is an ESP32-S3 robot with animated OLED eyes, a push-to-talk button, and a hardware mute switch. It's designed to connect to your PC over USB and help with tasks you approve, such as checking a project's Git status.

## Repositories

| Repository | What it contains |
| --- | --- |
| [moby-firmware](https://github.com/mobyuz/moby-firmware) | ESP32-S3 firmware and microphone bench tests. |
| [3d-model](https://github.com/mobyuz/3d-model) | Blender models, parts list, and wiring. |
| [moby-api](https://github.com/mobyuz/moby-api) | Rust backend for accounts, consent, AI, and voice. |
| [moby-web](https://github.com/mobyuz/moby-web) | Project website built with React and TypeScript. |

**Prototype in development.** Hardware testing and end-to-end Windows voice integration are next.
