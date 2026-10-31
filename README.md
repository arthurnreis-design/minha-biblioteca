Minha Biblioteca v4.5 — posições de leitura

- Substitui percentuais de leitura por posições (Posição X de Y) no leitor, Biblioteca, detalhes e Continue lendo.
- Armazena o mapa de posições de cada EPUB em uma nova tabela IndexedDB, para reutilização após fechar e reabrir.
- Preserva CFIs, destaques, anotações, marcadores e os dados existentes.
- O mapa é gerado na primeira abertura de cada EPUB após a atualização; isso pode levar algum tempo.
- As posições são unidades internas do EPUB, não páginas físicas, e podem permanecer iguais em páginas próximas.
- Não desinstale nem limpe os dados do aplicativo.
