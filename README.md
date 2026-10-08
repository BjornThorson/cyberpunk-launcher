# DECK/OS — Cyberpunk Launcher

An industrial cyberdeck-inspired **Android launcher design prototype**. This repository currently contains a mobile-first web prototype, not an installable Android home-screen replacement.

## Prototype features
- Four configurable quick-access modules (saved in local browser storage)
- Local clock and date
- Compact telemetry with honest browser capability fallbacks
- Command entry with module search and deterministic commands
- Module registry with search and swipe-up access
- Responsive industrial amber/cyan interface

## Run
Open `index.html` in a browser or serve the directory with `python3 -m http.server 8080`.

## Commands
`help`, `status`, `modules`, `config`, `clear`, `open web`, or a module name.

## Scope and limitations
Browser security prevents this prototype from discovering or launching arbitrary installed Android apps. Some module actions are placeholders. Battery data is shown only when the browser exposes it; connectivity reflects browser online state, not verified internet access. The eventual native Android launcher will use Kotlin/Jetpack Compose and Android launcher APIs.

## Design principles
- Functional industrial instrumentation, not decorative fake diagnostics
- Touch-first hybrid console with optional command navigation
- Predictable panel placement and accessible controls
- Shared action model for modules and terminal
