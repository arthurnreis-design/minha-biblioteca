Minha Biblioteca v6.9.38 — correção pontual do destaque de capítulo

Atualização do GitHub Pages: substitua index.html e sw.js (demais arquivos permanecem iguais).

Correção: a lista Capítulos resumidos passa a identificar a seção atual diretamente da localização do leitor EPUB, sem depender exclusivamente do parser CFI. Destaque visual neutro, cinza, consistente com a identidade atual. Sincronização resumo → EPUB e demais funções preservadas.

Teste: abra o EPUB em Aquém do bem e do mal, toque em IA e abra Capítulos resumidos; confirme a marcação No livro. Teste outro capítulo.

Observação: em EPUBs com vários capítulos dentro do mesmo arquivo interno, a identificação exata por âncora pode exigir tratamento adicional.
