# Site principal (eusougustavosampaio.com) — estado

Atualizado em 07/11/2026.

## Onde parei

No ar em `ead59b9`. O card do Método CIS abre o WhatsApp do comercial com "tenho interesse no Método CIS"; o do Homens de Honra leva à LP `/homensdehonra/`, e a arte já diz 12 de dezembro.

## Feito

- 05/11: página leve no celular (nota do Lighthouse de 70 para 92–96; peso de 12 MB para 442 KB), imagens em WebP.
- 06/11: prévia borrada embutida no HTML para a foto do topo e para os 7 banners; a foto só aparece quando está completa.
- 06/11: celular até 480 px baixa `assets/hero-mobile.webp` (51 KB, só o recorte que o celular mostra) no lugar da foto inteira (70 KB).
- Conferido: prints antes e depois idênticos em 375, 412 e 1440 px; sem JavaScript a foto aparece direto.
- 07/11: CIS → WhatsApp do comercial (o evento de outubro passou); Homens de Honra → `/homensdehonra/`; arte do HH com 12/12 (o "05" virou "12" em Bebas Neue, a fonte da arte).
- Publica por push no `master` (Workers Builds, worker `site-gks`).

## Falta / ideias

- Cache do navegador segue `max-age=0`: o build só copia `index.html`, `styles.css` e `assets`, então um `_headers` não sobe. Para ligar cache, mudar o build command na Cloudflare.

Nota no Cerebro: `Cerebro/03 - Projetos/Site Principal - Gustavo Sampaio.md`.
