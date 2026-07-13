# Troubleshooting

## Workflow falha com "Resource not accessible by integration"

**Causa**: Permissões insuficientes do GITHUB_TOKEN.

**Solução**: Vá em Settings → Actions → General → Workflow permissions → "Read and write permissions"

## Workflow falha com "Bad credentials"

**Causa**: Token expirado ou inválido.

**Solução**: Renove o `METRICS_TOKEN` em Settings → Developer settings → Personal access tokens.

## SVG não é atualizado

**Causa**: Workflow não executou ou falhou.

**Solução**: Vá em **Actions**, selecione o workflow "GitHub Metrics" e clique em **Run workflow**.

## Overview não aparece no perfil

**Causa**: Caminho incorreto ou SVG não gerado.

**Solução**:
1. Execute o workflow manualmente
2. Verifique se o arquivo `metrics/overview.svg` foi gerado
3. Confirme que o caminho no README está correto
