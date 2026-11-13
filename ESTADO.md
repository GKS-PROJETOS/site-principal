# Site principal (eusougustavosampaio.com) — estado

Atualizado em 13/11/2026.

## Onde parei

No ar em `165e9fc`. A home foi padronizada: topo só com "GUSTAVO SAMPAIO" (Urbanist, SAMPAIO em dourado) e os ícones das redes, e as 7 artes da vitrine no mesmo modelo (fundo grafite, foto à direita, dourado `#EBCB6C`). O Danilo quer passar página por página lapidando — tarefa no ClickUp `1dfmceyx0px`.

## Feito

- 05/11: página leve no celular (Lighthouse 70 → 92–96), imagens em WebP.
- 06/11: prévia borrada para a foto do topo e os banners; celular baixa `hero-mobile.webp`.
- 13/11: 7 artes novas com fotos do Drive da GKS, geradas pelo script em `~/projetos/gks/Referencia/site-principal-imagens-13-11/gerar-banners.py` (lista das fotos em `fotos-do-drive.json`). Linha dourada em cima, título, frase; eventos com data grande (PDA 23/01, HH 12/12). Sem "Saiba mais".
- 13/11: ordem da vitrine: Poder da Ação, Palestras, Treinamento Empresas, Homens de Honra, Mentoria, Método CIS, Contato.
- 13/11: borda dos cards em fio dourado; toque sem realce azul e sem zoom grudado.
- 13/11: cache de 1 ano para `assets/*` e `styles.css` (`_headers`), endereços com `?v=`. O build command na Cloudflare passou a copiar o `_headers`.
- 13/11: rodapé padrão de todos os sites (`.rodape-gs`).
- Backup da vitrine antiga: tag `backup-vitrine-2026-11-13`.
- Publica por push no `master` (Workers Builds, worker `site-gks`). Se o build travar ("internal error"), montar o `dist` e rodar o `wrangler deploy` do README.

## Falta / ideias

- **Trocou imagem, fonte ou CSS: mudar o `?v=` em todos os endereços** (index.html e styles.css), senão quem já visitou vê o antigo.
- Testar texto alternando de lado nos cards (ideia do Danilo).
- O local do Poder da Ação na arte diz só "Goiânia" até a produção confirmar.

Nota no Cerebro: `Cerebro/03 - Projetos/Site Principal - Gustavo Sampaio.md`.
