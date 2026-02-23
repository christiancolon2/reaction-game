REACTION.IO // Professional Reaction Timer

A high-performance, interactive reaction benchmarking tool built with vanilla JavaScript and Three.js. This project was designed to demonstrate core frontend competencies: millisecond-precise timing, low-latency audio processing, and state-driven 3D animations.

🚀 Live Demo

🚀 Live Demo

[https://christiancolon2.github.io/reaction-game/](https://christiancolon2.github.io/reaction-game/)

📸 Screenshots

[View screenshots](./screenshots/)

🛠️ Tech Stack

Engine: Vanilla JavaScript (ES6+)

Graphics: Three.js (WebGL)

Audio: Web Audio API (Low-latency Oscillators)

Styling: CSS3 (Modern Flexbox/Grid, Backdrop Filters, Custom Properties)

Data: LocalStorage API for persistent session tracking

✨ Key Features

1. High-Precision Timing

Unlike standard Date.now(), this application utilizes performance.now(). This provides sub-millisecond resolution and is immune to system clock drift, ensuring the most accurate reflex measurement possible.

2. Reactive 3D Visualization

The central Torus Knot is not merely decorative; it is a visual state indicator.

Idle: Slow, soothing emerald pulse.

Waiting: High-frequency vibration and desaturation.

Ready: Instant emission burst and high-speed rotation.

Error: Red-shifted violent shake for false starts.

3. Low-Latency Web Audio

To minimize the "input-to-audio" delay found in standard HTML5 <audio> tags, this project implements the Web Audio API. It generates sine and sawtooth waveforms on the fly using oscillators, providing instant audible cues for triggers and errors.

4. Accessibility & UX

Keyboard Support: Complete game loop controllable via the Spacebar.

Cheat Detection: False-start logic with immediate UI/3D feedback.

Mobile Optimized: Fluid layouts and touch-event handling.

Performance Index: Contextual feedback based on human reflex averages.

📊 Performance Index

Rating

Criteria

Superhuman

< 200ms

Excellent

200ms - 279ms

Good

280ms - 349ms

Average

350ms - 449ms

Below Average

450ms+

🏗️ Architecture & Decisions

State Management: Implemented via a centralized Game class that coordinates the UI, Audio, and 3D Scene states.

Zero Dependencies: Built without frameworks to showcase mastery of the Document Object Model (DOM) and browser APIs.

Flicker-Free Reset: Replaced full-page reloads with a soft-reset logic to maintain the WebGL context and provide a seamless user experience.

🔧 Installation

Since this is a static site, no build tools or installation are required.

Clone the repository.

Open index.html in any modern evergreen browser.

Created as a technical portfolio project for Frontend Engineering roles.
