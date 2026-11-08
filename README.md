# Minha Biblioteca v6.9.41 — correção da geração de resumos

## Mudanças
- Worker: segunda tentativa de resumo revisa o rascunho anterior em relação ao capítulo original, com meta explícita de palavras e recuperação de cenas omitidas; limite de 2 tentativas para evitar repetição de custos.
- Aplicativo: erro de geração continua visível após encerramento, em vez de ser substituído por “Processamento encerrado”.
- Validação de extensão permanece ativa: nenhum resumo fora da faixa é salvo automaticamente.
- Demais ferramentas de IA e interface preservadas.

## Publicação
1. Faça backup do Worker atual. Copie todo o conteúdo de `worker_cloudflare_para_copiar.txt` para o editor do Worker no Cloudflare e publique. Preserve Secrets e Variables.
2. No GitHub Pages, substitua `index.html` e `sw.js`.
3. Reabra a Minha Biblioteca e teste um capítulo no modo Narrativo condensado.

## Limitações
A integração com a OpenAI não foi testada com a conta do usuário. A extensão é um controle objetivo, mas não comprova fidelidade narrativa. Se a IA não atingir a faixa, a geração falhará com mensagem visível, sem salvar um resumo inadequado. A segunda tentativa pode gerar custo adicional.
