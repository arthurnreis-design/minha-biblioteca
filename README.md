# Minha Biblioteca v6.9.36 — Progresso e páginas

Atualização apenas da PWA no GitHub Pages. **Não alterar o Cloudflare Worker.**

- Cards Continuar lendo: coluna de informações alinhada ao topo da capa, percentual de progresso calculado pela posição atual/total, barra com contraste adaptativo e páginas estimadas.
- Detalhes do livro: total de páginas estimadas e lista expansível de estimativas por capítulo (quando o EPUB permite identificar as seções).
- Leitor de resumos: remoção dos eventos de toque antigos ao recalcular a paginação na ampliação, evitando que um toque avance duas páginas. Swipe preservado.
- Páginas são estimadas com base nas posições EPUB.js (~150 caracteres por posição; referência de 1.800 caracteres por página), não correspondem necessariamente à paginação editorial.
- Não foi alterado o percentual dentro do leitor EPUB nem o progresso independente dos resumos.

Publique index.html e sw.js no GitHub e teste em seu Samsung. Faça backup da versão anterior e dos dados antes de atualizar.
