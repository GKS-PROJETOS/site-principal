# site-principal

Site institucional publicado em www.eusougustavosampaio.com

## Deploy

O deploy e automatico via Cloudflare Workers Builds.
Todo push no branch master dispara um build e publica o worker site-gks.

Build command:
rm -rf dist && mkdir dist && cp -r index.html styles.css assets dist/

Deploy command:
npx wrangler deploy --name site-gks --assets ./dist --compatibility-date 2026-08-17

Nao e mais necessario subir arquivos manualmente no painel da Cloudflare.
