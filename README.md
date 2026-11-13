# site-principal

Site institucional publicado em www.eusougustavosampaio.com

## Deploy

O deploy e automatico via Cloudflare Workers Builds.
Todo push no branch master dispara um build e publica o worker site-gks.

Build command:
rm -rf dist && mkdir dist && cp -r index.html styles.css assets dist/ && if [ -f _headers ]; then cp _headers dist/; fi

Deploy command:
npx wrangler deploy --name site-gks --assets ./dist --compatibility-date 2026-08-17

Nao e mais necessario subir arquivos manualmente no painel da Cloudflare.

## Cache (desde 13/11/2026)

O `_headers` guarda `assets/*` e `styles.css` por 1 ano no aparelho. Todo endereco de
arquivo no `index.html` e no `styles.css` leva `?v=AAAAMMDD`. **Trocou uma imagem, a fonte
ou o CSS? Mude o `v` (em todos os lugares)**, senao quem ja visitou continua vendo o antigo.
