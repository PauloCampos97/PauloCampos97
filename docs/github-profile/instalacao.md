# Instalação

## 1. Fork/Clone o repositório

```bash
git clone https://github.com/PauloCampos97/PauloCampos97.git
cd PauloCampos97
```

## 2. Crie os secrets no GitHub

Vá em: **Settings → Secrets and variables → Actions**

Crie:
- `METRICS_TOKEN` - Fine-grained PAT
- `WAKATIME_API_KEY` - API key do WakaTime

## 3. Configure permissões dos workflows

**Settings → Actions → General → Workflow permissions**: Selecione "Read and write permissions"

## 4. Execute manualmente

Acesse a aba **Actions** e execute:
1. GitHub Metrics → Run workflow
2. Generate Snake → Run workflow
3. WakaTime Metrics → Run workflow

## 5. Verifique os resultados

Após a execução, os SVGs estarão em `metrics/` e a snake em `github-contribution-grid-snake.svg`.
