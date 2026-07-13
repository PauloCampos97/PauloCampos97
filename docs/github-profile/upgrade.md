# Upgrade

## lowlighter/metrics

O workflow usa `lowlighter/metrics@latest`. Para verificar atualizações:

1. Acesse [github.com/lowlighter/metrics/releases](https://github.com/lowlighter/metrics/releases)
2. Verifique breaking changes no CHANGELOG
3. Para fixar uma versão específica, troque `@latest` pela tag desejada

## Platane/snk

O workflow usa `Platane/snk@v3`. Para verificar atualizações:

1. Acesse [github.com/Platane/snk/releases](https://github.com/Platane/snk/releases)
2. A major version v3 garante compatibilidade
3. Para usar a versão mais recente, troque `@v3` por `@v4` quando disponível

## Como verificar breaking changes

1. Leia o release notes de cada nova versão
2. Verifique as issues do repositório para problemas conhecidos
3. Execute o workflow manualmente para testar antes do próximo cron

## Script de validação

Verifique manualmente:
- YAML syntax: `yamllint .github/workflows/*.yml`
- Markdown: Previsualize no VS Code
- Links: Clique em cada link no README
- SVGs: Confira se os arquivos foram gerados na raiz
