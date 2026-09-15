# Aula 4 — Primeiros Passos em Redes: IP e Conectividade

## O que aprendi

- Todo dispositivo conectado a uma rede tem um endereço IP, que funciona como identificador único enquanto está conectado.
- O comando `ping` testa se é possível alcançar outro dispositivo ou servidor, medindo o tempo de ida e volta de um pacote de dados.

## Comandos praticados

| Comando | Função |
|---|---|
| `ipconfig` | Mostra o IP do computador e outras informações de rede |
| `ping [endereço]` | Testa conectividade com um destino (ex: `ping google.com`) |

## Conceitos que comecei a explorar

- **Gateway padrão**: é o IP do roteador, a "porta de saída" da rede local para a internet.
- **Máscara de sub-rede**: define quais dispositivos pertencem à mesma rede local.

## Lição principal

Tempo de resposta do `ping` baixo (10-50ms) indica rede rápida; tempo alto (300ms+) indica possível problema de rede. Isso é o primeiro passo de qualquer troubleshooting de conectividade.
