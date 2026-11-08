# Minha Biblioteca v6.9.34 — melhorias de leitura e navegação

Atualize no GitHub: index.html, sw.js e, opcionalmente, este README.md.

**Não atualize o Cloudflare Worker.** O worker.js do pacote é uma cópia inalterada da v6.9.33 e não deve ser publicado no GitHub.

## Principais mudanças
- Tela de geração: somente capítulos sem resumo, ocultação e restauração por livro, linhas compactas.
- Tela separada de capítulos resumidos, com leitura individual e leitura sequencial.
- Geração individual abre o resumo diretamente após salvar.
- Correção da posição ao voltar do dicionário e toque lateral no leitor paginado.
- Acesso Início na leitura e na lista de resumos.
- Continuar resumo no cartão inicial, mantendo progresso separado do EPUB.
- Removida seção Último destaque; mantidos contadores.
- Padronização visual do cabeçalho EPUB, destaque suave na IA e atualização de menus/carregamento.

## Cuidados
- Faça backup de dados no aplicativo e guarde a v6.9.33 antes de atualizar. O backup do aplicativo não inclui os arquivos EPUB.
- Teste primeiro um livro, especialmente leitura do resumo, dicionário, modo ampliado e navegação Início.
- A retomada de resumos salva capítulo e página/posição proporcional. Se o tamanho da tela ou a fonte mudar, a mesma página pode não corresponder exatamente à mesma palavra.
- A navegação para marcações do EPUB utiliza o mecanismo de consulta temporária existente para retornar à posição anterior.
