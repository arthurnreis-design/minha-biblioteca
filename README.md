# Minha Biblioteca v6.9.40 — IA integrada

## Publicação (uma única atualização do Cloudflare)
1. Faça backup do Worker atual no painel Cloudflare antes de alterar.
2. Abra o Worker `minha-biblioteca-ia` > Editar código, substitua pelo conteúdo COMPLETO de `worker_cloudflare_para_copiar.js` e publique uma vez. NÃO altere os secrets `OPENAI_API_KEY` e `APP_ACCESS_TOKEN` nem o endereço do Worker.
3. No GitHub Pages, atualize `index.html` e `sw.js` (os ícones e o manifest não precisam ser trocados). Reabra o PWA para carregar o novo cache.

## Novidades
- Resumos: três modalidades mantidas, alvo explícito de extensão, até três tentativas automáticas quando a redução fica fora da faixa; se falhar, não salva um resultado fora do padrão. Isso pode aumentar custo e tempo. Para capítulos com menos de 180 palavras não é aplicada a faixa de palavras.
- Leitor EPUB e leitor de resumos: selecionar trecho > Explicar IA / Contexto histórico / Traduzir IA. Consulta online, sem mudar a posição salva.
- Descobrir livros: botão `Sugestões IA` opcional; a IA gera termos de busca, e as recomendações só aparecem após confirmação de edição em português na Open Library. O botão de atualização tradicional permanece.

## Limitações e segurança
- Não há garantia matemática de fidelidade narrativa nem de percentuais exatos. O controle de extensão rejeita resultados discrepantes, mas não substitui avaliação humana do conteúdo.
- Consultas de IA e novas tentativas podem consumir tokens pagos. Os textos selecionados e os títulos usados nas sugestões são enviados à OpenAI via Worker.
- O app não tem pesquisa histórica em tempo real na IA; contextualização pode conter imprecisões, portanto é necessário verificar fatos importantes.
- Não há alterações nos livros salvos, nos resumos existentes ou no IndexedDB. Resumos antigos de 92% não são corrigidos automaticamente.
- Validação local: sintaxe JS e simulação do Worker; não foram feitos testes de ponta a ponta com sua chave ou seu EPUB.
