# Tokens e Secrets

## METRICS_TOKEN

Token de acesso pessoal para ler dados do GitHub. Utilizado pelo workflow `metrics.yml`.

### Como criar

1. Acesse: **Settings → Developer settings → Personal access tokens → Fine-grained tokens**
2. Clique em **Generate new token**
3. Configure:
   - **Token name**: `METRICS_TOKEN`
   - **Expiration**: No expiration
   - **Repository access**: Only select repositories → `PauloCampos97`
   - **Permissions**:
     - Contents: Read and write
     - Metadata: Read-only
     - Issues: Read-only
     - Pull requests: Read-only
4. Gere o token e copie-o

### Como salvar

1. Vá em: **Settings → Secrets and variables → Actions**
2. **New repository secret**
3. Nome: `METRICS_TOKEN`
4. Valor: cole o token gerado
5. Salve

## GITHUB_TOKEN

Token automático fornecido pelo GitHub Actions. Utilizado pelo workflow `snake.yml` para fazer commit dos SVGs gerados. Não precisa configurar.

**Nunca coloque tokens diretamente nos arquivos YAML.**

Sempre utilize `${{ secrets.NOME_DO_SECRET }}`.
