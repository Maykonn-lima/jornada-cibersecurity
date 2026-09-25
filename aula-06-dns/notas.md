# Aula 6 — DNS na Prática

## O que aprendi

- DNS é o sistema que traduz nomes de sites em endereços IP.
- Sites grandes (Google, GitHub) usam vários servidores espalhados pelo mundo (CDN), então o IP retornado pode variar dependendo de onde e quando se testa.

## Comando praticado

| Comando | Função |
|---|---|
| `nslookup [site]` | Mostra o IP por trás de um nome de site |

## Teste realizado

Testei `nslookup github.com` duas vezes seguidas — o IP retornado foi o mesmo (`4.228.31.150`) nas duas vezes, já que o teste foi feito no mesmo local e momento.

## Lição principal para troubleshooting

- Se o `ping` funciona mas o `nslookup` não retorna nada → problema específico de DNS.
- Se nem o `ping` funciona → problema mais geral de conectividade, não só de DNS.
