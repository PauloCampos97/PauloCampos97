# Upgrade

## lowlighter/metrics

O workflow `metrics.yml` usa `lowlighter/metrics@latest`. Para verificar atualizações:

1. Acesse [github.com/lowlighter/metrics/releases](https://github.com/lowlighter/metrics/releases)
2. Verifique breaking changes no CHANGELOG
3. Para fixar uma versão específica, troque `@latest` pela tag desejada

## Platane/snk

O workflow `snake.yml` usa `Platane/snk/svg-only@v3`. Para verificar atualizações:

1. Acesse [github.com/Platane/snk/releases](https://github.com/Platane/snk/releases)
2. Verifique breaking changes no release notes
3. Para fixar uma versão específica, altere a tag `@v3` para a versão desejada

## Como verificar breaking changes

1. Leia o release notes de cada nova versão
2. Verifique as issues do repositório para problemas conhecidos
3. Execute o workflow manualmente para testar antes do próximo cron

## Validação

Verifique manualmente:

- **YAML**: Os arquivos `.github/workflows/metrics.yml` e `.github/workflows/snake.yml` estão sintaticamente corretos
- **Markdown**: Pré-visualize o README no VS Code
- **Links**: Clique em cada link no README para confirmar que funcionam
- **SVGs**: Confira se os SVGs foram gerados corretamente:
  - `metrics/overview.svg`
  - `metrics/extras.svg`
  - `assets/snake-dark.svg`
  - `assets/snake-light.svg`
