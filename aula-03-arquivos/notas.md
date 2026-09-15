# Aula 3 — Criar e Apagar Arquivos e Pastas

## O que aprendi

- É possível criar pastas e arquivos vazios diretamente por comando.
- O sistema protege contra exclusão acidental de pastas com conteúdo, pedindo confirmação.

## Comandos praticados

| Comando | Função |
|---|---|
| `mkdir [nome]` | Cria uma pasta nova |
| `New-Item [nome].txt` | Cria um arquivo vazio |
| `del [nome]` | Apaga um arquivo (sem aviso) |
| `rmdir [nome]` | Apaga uma pasta (só direto se estiver vazia) |

## Desafio resolvido

Tentei apagar uma pasta com arquivo dentro usando `rmdir` — o sistema pediu confirmação, avisando que os "filhos" (conteúdo) seriam removidos junto. Isso me ensinou que apagar por comando não vai para a Lixeira, então o sistema avisa antes.

## Ordem correta para apagar pasta com conteúdo

1. Entrar na pasta (`cd [pasta]`)
2. Apagar os arquivos de dentro primeiro (`del [nome]`)
3. Sair (`cd ..`)
4. Só então apagar a pasta vazia (`rmdir [nome]`)
