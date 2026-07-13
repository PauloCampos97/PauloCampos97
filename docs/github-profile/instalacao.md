# Instalação

## 1. Fork/Clone o repositório

```bash
git clone https://github.com/PauloCampos97/PauloCampos97.git
cd PauloCampos97
```

## 2. Crie os secrets no GitHub

Vá em: **Settings → Secrets and variables → Actions**

Crie:
- `METRICS_TOKEN` — Fine-grained PAT com permissões de leitura e escrita

## 3. Configure permissões dos workflows

**Settings → Actions → General → Workflow permissions**: Selecione "Read and write permissions"

## 4. Execute manualmente

Acesse a aba **Actions** e execute cada workflow:

1. **GitHub Metrics** → Run workflow (gera `metrics/overview.svg` e `metrics/extras.svg`)
2. **Generate Snake** → Run workflow (gera `assets/snake-dark.svg` e `assets/snake-light.svg`)

## 5. Verifique os resultados

Após a execução, os seguintes arquivos serão gerados:

| Workflow | Saída |
|---|---|
| metrics.yml (job: overview) | `metrics/overview.svg` |
| metrics.yml (job: extras) | `metrics/extras.svg` |
| snake.yml | `assets/snake-dark.svg` e `assets/snake-light.svg` |
