# Minha Biblioteca v6.9.33 — Integração com IA

1. Faça backup dos dados no app atual (não inclui EPUBs).
2. No Cloudflare, substitua o código do Worker `minha-biblioteca-ia` pelo conteúdo de `worker.js`. Mantenha os Secrets `OPENAI_API_KEY` e `APP_ACCESS_TOKEN` sem copiá-los para o GitHub.
3. Opcional: configure as variáveis `MODEL` (`gpt-5.4-mini`), `INPUT_USD_PER_MILLION` e `OUTPUT_USD_PER_MILLION` com os preços atuais do modelo. Sem as tarifas, o custo efetivo aparecerá como não calculado; os tokens serão registrados.
4. Publique no GitHub apenas `index.html`, `sw.js`, `manifest.webmanifest` e os ícones. **NÃO publique `worker.js` no GitHub.**
5. Abra a PWA, vá a Ajustes > Inteligência artificial > Configurar acesso à IA, insira o valor de APP_ACCESS_TOKEN.
6. Teste primeiro um capítulo curto e o preenchimento inteligente; depois a seleção múltipla.

A geração sequencial processa um capítulo por vez e interrompe no primeiro erro. A seleção e o estilo são temporários. O consumo fica armazenado localmente.

A estimativa exibida antes da geração usa tarifas ilustrativas e não é uma cotação oficial. O histórico de custo real estimado só será preenchido se as tarifas forem configuradas no Worker.
