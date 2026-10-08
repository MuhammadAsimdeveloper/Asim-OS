# Asim Tools Module Plan — Asim-OS

Date: 2026-10-08

## Role
local/offline OS utilities and services

## Rule
These are **backend modules to copy locally**, not a remote tool service. Do not call, iframe, link, or fetch Asim Tools at runtime. Do not add a standalone Tools page/section. Integrate the copied functionality into this repository's existing backend or service layer.

## Assigned modules
### Text


### Developer


### Calculators


### Security


### Images


### Time


### Data & Developer


### Converters


### Documents & PDF


### Networking & Web


### Student & Science


### AI & Agents


### Build & Package


## Implementation sequence
1. Copy the smallest needed module and its focused tests.
2. Adapt imports/types/error handling to this repository.
3. Register the helper in the existing service layer.
4. Add repository-native tests before exposing the behavior.
5. For network tools, retain explicit target validation/privacy/rate-limit boundaries.
6. For EXTRACT-FIRST tools, wait for the canonical backend extraction from Asim Tools; do not copy DOM/UI behavior from `src/app.js`.
