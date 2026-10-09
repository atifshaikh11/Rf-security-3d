# RF Security Monitoring — 3D Digital Twin

A browser-based Three.js prototype for the FYP **“Joint Open-Set Signal-Type and Device Identification for Low-Cost SDR-Based RF Security Monitoring.”** It uses procedural geometry rather than external 3D model downloads.

## Requirements
- Node.js 20 or newer
- npm

## Run locally
```bash
npm install
npm run dev
```
Open the local URL printed by Vite (usually `http://localhost:5173`).

## Included
- Orbit/zoom/pan 3D lab scene with procedural ESP32 + CC1101 transmitter boards, antennas, RTL-SDR receiver, laptop, and optional Raspberry Pi.
- Animated RF rings and moving data particles.
- Play/pause/reset, step mode, scenario controls, camera presets, modulation display, and fingerprint drift illustration.
- Three demonstration scenarios: known Device A, unknown/unregistered device, and unknown signal type.
- Explicit simulation-only labels and a Live Hardware state that truthfully reports the backend is not connected.

## Scientific boundary
This is an **interactive visual simulation**, not a measured RF propagation model or a connected SDR/AI backend. Scores and outcomes are demo values. The current prototype does not acquire IQ samples, train/run a CNN, or infer actual device identity. A real hardware mode requires a separate backend to acquire RTL-SDR IQ data and connect the implemented inference pipeline.
