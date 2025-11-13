# openai-actions-policies

Dette repoet inneholder personvernerklæringer og relaterte policy-dokumenter
for GPT Actions og API-integrasjoner.

Repoet er satt opp for å bli publisert via **GitHub Pages**, slik at hver
HTML-fil kan brukes som en offentlig, HTTPS-basert URL i OpenAI GPT Actions.

## Struktur

- `index.html`  
  Landing-side med oversikt over tilgjengelige policy-dokumenter.

- `privacy-generic-no.html`  
  Generisk personvernerklæring (norsk) for GPT Actions.

- `privacy-generic-en.html`  
  Generisk personvernerklæring (engelsk) for GPT Actions.

- `privacy-example-action-no.html`  
  Eksempel på en spesifikk personvernerklæring for én GPT Action (norsk).
  Kopier denne når du lager nye Actions.

## Bruk med GitHub Pages

1. Gå til **Settings → Pages** i dette repoet.
2. Under “Build and deployment”:
   - Source: `Deploy from a branch`
   - Branch: f.eks. `main` og rotmappe `/`.
3. Trykk **Save**.

Når GitHub Pages er aktiv, vil du få en URL som:

`https://<brukernavn>.github.io/openai-actions-policies/`

Eksempler:

- Generisk personvern (NO):  
  `https://<brukernavn>.github.io/openai-actions-policies/privacy-generic-no.html`

- Generisk personvern (EN):  
  `https://<brukernavn>.github.io/openai-actions-policies/privacy-generic-en.html`

Disse URL-ene kan du lime inn som **Privacy policy URL** i OpenAI GPT Actions.
