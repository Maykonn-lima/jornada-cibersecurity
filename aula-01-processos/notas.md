# Aula 1 — Processos e Linha de Comando (PowerShell)

## O que aprendi

- Um **processo** é qualquer programa em execução (cada aba do navegador é um processo separado).
- **PID** é um número único e temporário que identifica um processo enquanto ele está ativo.
- "Matar" um processo significa forçar seu encerramento, sem chance de salvar dados.

## Comandos praticados

| Comando | Função |
|---|---|
| `tasklist` | Lista todos os processos rodando |
| `get-process` | Lista processos (sintaxe PowerShell) |
| `get-process [nome]` | Filtra por nome |
| `stop-process -id [PID] -force` | Encerra um processo pelo PID |

## Erros que cometi (e o que aprendi)

1. `taskill` → erro, faltou um "k". Certo é `taskkill` (no CMD) ou `stop-process` (no PowerShell).
2. `stop-process -id 10016` → erro "processo não encontrado". PID já não existia mais — aprendi que PIDs são dinâmicos.
3. `set-process chrome` → comando não existe. O certo é `stop-process`.

## Lição principal

Antes de agir sobre um processo, sempre confirmar seu estado atual com `get-process` — nunca confiar em PID antigo.
