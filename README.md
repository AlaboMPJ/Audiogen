# Sonagen: prompt-to-audio studio

A minimal Next.js studio that turns a written prompt plus synthesis parameters into freshly rendered audio. A clean, typed example of wiring a generative audio model into a usable product surface.

## What it demonstrates

- Generative audio integration: the `/api/generate-sound` route talks to OpenAI's audio-preview models or Stability's Stable Audio, behind one interface.
- Provider-agnostic design: the audio backend is swappable without touching the UI.
- Product-quality frontend: prompt composer, parameter controls, waveform and playback, status and toast feedback, all typed end to end.

## Stack

- Next.js (App Router), TypeScript, Tailwind.
- OpenAI / Stability audio APIs behind a single provider interface.

## Run it

```bash
npm install
# add the providers you want to .env.local (see .env.example):
#   OPENAI_API_KEY=...        for gpt-4o-audio-preview
#   STABILITY_API_KEY=...     for Stable Audio
npm run dev
```

Open http://localhost:3000, write a prompt, set the parameters, and render.

## Notes

A focused build to show clean generative-AI integration: a single typed API boundary, swappable providers, and a UI that makes the model usable.
