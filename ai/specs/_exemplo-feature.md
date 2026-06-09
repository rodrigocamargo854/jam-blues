# Spec: Timer Global

## O que faz
Timer global para controlar a duração total da rotina diária; permite iniciar, pausar e resetar, exibindo tempo decorrido e label de estado.

## Fluxo
1. Usuário clica em `INICIAR` → timer começa a contar e o botão vira `PAUSAR`.
2. Enquanto o timer roda, eventos internos disparam (ex.: mudança de bloco quando tempo do bloco termina).
3. Usuário pode `RESET` para voltar ao estado inicial (00:00) e limpar labels.

## Critérios de aceite
- Timer conta segundos corretamente (incremento a cada 1s) mesmo com múltiplos blocos.
- Botões `INICIAR`, `PAUSAR` e `RESET` refletem estado atual e são acessíveis via teclado.
- Timer reseta corretamente e libera recursos (clearInterval) para evitar múltiplos timers ativos.
