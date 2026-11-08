# Minha Biblioteca v6.9.37

Atualização incremental sobre a v6.9.36.

## Alterações
- Ao abrir um capítulo com resumo salvo, a posição do EPUB acompanha o início do capítulo correspondente, inclusive ao voltar para capítulos anteriores.
- A lista **Capítulos resumidos** destaca discretamente o capítulo correspondente à posição atual do EPUB, com a etiqueta **No livro**.
- Mantém a página exata de leitura dos resumos separada da posição do EPUB.
- Mantém o progresso do EPUB baseado nas posições existentes. Quando disponível, usa o mapa de posições já armazenado para atualizar o indicador sem recalcular o EPUB.

## Instalação
Substitua `index.html` e `sw.js` no GitHub Pages. Os demais arquivos do pacote são preservados sem alterações. Não é necessário alterar o Cloudflare Worker.

## Testes sugeridos
1. Abra um resumo do capítulo 10 e confirme que **Continuar livro** leva ao início desse capítulo.
2. Abra um resumo anterior e depois volte ao 10, conferindo se o progresso acompanha ambos.
3. Dentro do EPUB, abra **Capítulos resumidos** e confira a etiqueta **No livro**.
4. Confirme que marcadores, notas e a página salva do resumo permanecem intactos.

Observação: a precisão da correspondência depende do índice fornecido pelo arquivo EPUB. Se o livro não tiver mapa de posições calculado, o percentual poderá ser atualizado ao abrir o leitor EPUB.
