# Minha Biblioteca v4.7 — atualização de interface e leitura

Atualização incremental sobre a versão v4.6. Os arquivos EPUB, fichas, anotações, marcadores e progresso continuam armazenados localmente no mesmo IndexedDB (`minha_biblioteca_v1`). **Não desinstale o aplicativo, não limpe os dados do navegador e não apague o armazenamento do site.** Antes de atualizar, use **Ajustes → Exportar dados** como precaução (o backup não inclui os arquivos EPUB).

## Alterações
- Biblioteca: cards de Autores, Séries e Coleções mais compactos, com até seis capas do mesmo tamanho; lista de livros com capas maiores; navegação Anterior/Próximo nos detalhes quando aberta a partir de um grupo, e retorno ao grupo.
- Favoritos independentes de Para ler depois, com estrela própria, marca discreta na capa e filtro.
- Status de leitura com nomes mais claros e chips de cores discretas; pausa/retomada somente para livros já iniciados; menu de filtros/ordenação compacto.
- Recomendações: tentativa de oferecer até 15 opções, preservando a busca de edições em português e sem garantir quantidade quando o catálogo não fornecer resultados; capas exibidas inteiras.
- Menu Aa: botões +/- e níveis para fonte e luminosidade; três opções visíveis de tema, fonte e espaçamento entre parágrafos. Espaçamento salvo por livro.
- Luminosidade uniforme em toda a tela do leitor, incluindo cabeçalho e rodapé; cor do título inspirada na capa (com fallback ao estilo original).
- Seleção de texto: barra própria mais discreta e posicionada abaixo da seleção; notas internas reconhecidas na seção atual podem abrir em janela rolável.
- Ficha do livro: preenchimento inteligente por copiar pedido e colar resposta estruturada, com prévia editável e confirmação antes de substituir informações.

## Limitações e cuidados
- **O indicador de posição não foi modificado** e continua somente informativo. Não há salto por número de posição.
- Notas e links variam entre EPUBs. A janela de nota funciona quando o destino está disponível no documento atual; links em outras seções podem continuar seguindo a navegação nativa do EPUB.
- A identidade do título usa extração simples de cor, não IA e não reprodução fiel do desenho da capa.
- O número de sugestões depende da disponibilidade de edições em português no catálogo externo e da rede.
- A verificação automática realizada cobre sintaxe JavaScript e integridade do pacote; o teste funcional completo em Samsung Internet com EPUBs reais ainda precisa ser feito no aparelho.

## Instalação
Substitua os arquivos do repositório GitHub Pages pelos arquivos deste ZIP, mantendo a mesma URL e a instalação existente. Aguarde a atualização do service worker e reabra o app. **Não limpe os dados do site.**
