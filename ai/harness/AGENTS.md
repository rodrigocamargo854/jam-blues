# Agents Context — Treino Matinal — Piano

## Como rodar
Abra `index.html` no navegador (duplo clique) ou sirva a pasta com um servidor estático. Exemplo:

```bash
npx serve .
# ou
python3 -m http.server 8000
```

## Estrutura do projeto
- `index.html` → interface principal, estilos e lógica do exercício.
- `ai/` → documentação, specs e arquivos para agentes e automatizações.

## Fluxo de dados
1. Usuário interage com a UI (seleciona bloco, inicia timer).
2. JavaScript atualiza display do teclado, metrônomo e timers.
3. A interface exibe sugestões, vídeos e marca exercícios como concluídos.

## O que não existe (ainda)
- Persistência de progresso do usuário (sem backend nem storage remoto).
- Contas de usuário ou sincronização entre dispositivos.
