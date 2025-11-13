# NORSAIN Privacy

Dette repoet er NORSAINs sentrale kilde for personvernerklæringer og relaterte
policy-dokumenter for digitale tjenester, inkludert GPT-baserte assistenter,
Actions og andre API-integrasjoner.

Koden publiseres som et statisk nettsted via **GitHub Pages**, og hver HTML-fil
kan brukes som en offentlig, HTTPS-basert URL i eksterne grensesnitt
(for eksempel OpenAI GPT Actions, web-applikasjoner eller dokumentasjon).

## Struktur

Alle publiserte sider ligger i `src/` og eksponeres på GitHub Pages:

- `src/index.html`  
  Landingsside med oversikt over tilgjengelige policy-dokumenter.

- `src/privacy-generic-no.html`  
  Generisk personvernerklæring (norsk) for NORSAIN-tjenester og GPT Actions.

- `src/privacy-generic-en.html`  
  Generisk privacy policy (engelsk) for NORSAIN services and GPT Actions.

- `src/privacy-example-action-no.html`  
  Eksempel på en spesifikk personvernerklæring for én GPT Action (norsk).
  Kopier denne som utgangspunkt når du lager nye Action-spesifikke policies.

Ved behov kan det legges til flere filer, for eksempel per produkt, per Action
eller per kunde/tenant.

## Publisering med GitHub Pages (GitHub Actions)

Repoet er satt opp til å bruke GitHub Pages via en GitHub Actions-workflow:

- Workflow: `.github/workflows/static.yml`
- Bygger og publiserer innholdet i `./src` ved push til `main`.

For å verifisere konfigurasjonen:

1. Gå til **Settings → Pages** i dette repoet.
2. Under **Build and deployment**, sett:
   - **Source**: `GitHub Actions`.

Når en workflow-kjøring har fullført, vil nettstedet være tilgjengelig på:

```text
https://norsain-ai.github.io/norsain-privacy/
