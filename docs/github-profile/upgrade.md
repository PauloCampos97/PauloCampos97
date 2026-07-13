# Upgrade

## lowlighter/metrics

O workflow usa `lowlighter/metrics@latest`. Para verificar atualizações:

1. Acesse [github.com/lowlighter/metrics/releases](https://github.com/lowlighter/metrics/releases)
2. Verifique breaking changes no CHANGELOG
3. Para fixar uma versão específica, troque `@latest` pela tag desejada

## Como verificar breaking changes

1. Leia o release notes de cada nova versão
2. Verifique as issues do repositório para problemas conhecidos
3. Execute o workflow manualmente para testar antes do próximo cron

## Validação

Verifique manualmente:
- **YAML**: O arquivo `.github/workflows/metrics.yml` está sintaticamente correto
- **Markdown**: Pré-visualize o README no VS Code
- **Links**: Clique em cada link no README para confirmar que funcionam
- **SVG**: Confira se `metrics/overview.svg` foi gerado corretamente
