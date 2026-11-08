# AventIQ V2.4

Next.js app with the AventIQ UI and the opportunity dataset at `src/data/opportunities.ts`.

## Run locally

```bash
npm install
npm run dev
```

## Build

```bash
npm run build
```

## Vercel

Import the repository with **Root Directory** set to `./` (repository root). The Next.js app entry point is `src/app/page.tsx`.

Deadlines that are exact ISO dates in the past are hidden by the discovery filter; rolling and non-date deadlines remain eligible to display. Verify details on each official source before applying.

## Added community and consultation features (prototype)

- Opportunity ratings and comments are added inside opportunity cards. They persist in the visitor's browser via `localStorage`; they are not shared across users and currently have no moderation/authentication backend.
- Consultation room creation is available in the Video calls section. Rooms open using Jitsi Meet in a new tab; share the generated room name with the other participant.
- Commission/payment processing is **not integrated**. A real paid consultation flow requires a payment provider, server-side booking/payment verification, commission calculation, secure user accounts, moderation, privacy/consent, and appropriate safeguards before launch. Do not collect payment based only on this prototype.
- Existing opportunity data file (`src/data/opportunities.ts`) and core discovery layout are retained.
