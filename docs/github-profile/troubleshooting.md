# Troubleshooting

## Workflow falha com "Resource not accessible by integration"

**Causa**: Permissões insuficientes do GITHUB_TOKEN.

**Solução**: Vá em Settings → Actions → General → Workflow permissions → "Read and write permissions"

## Workflow metrics.yml falha com "Bad credentials"

**Causa**: Token expirado ou inválido.

**Solução**: Renove o `METRICS_TOKEN` em Settings → Developer settings → Personal access tokens.

## SVGs não são atualizados

**Causa**: Workflow não executou ou falhou.

**Solução**: Vá em **Actions**, selecione o workflow desejado (GitHub Metrics ou Generate Snake) e clique em **Run workflow**.

## Overview ou Extras não aparecem no perfil

**Causa**: Caminho incorreto ou SVG não gerado.

**Solução**:
1. Execute o workflow `GitHub Metrics` manualmente
2. Verifique se os arquivos `metrics/overview.svg` e `metrics/extras.svg` foram gerados
3. Confirme que os caminhos no README estão corretos

## Snake não aparece no perfil

**Causa**: Workflow snake.yml não executou ou o caminho está incorreto.

**Solução**:
1. Execute o workflow `Generate Snake` manualmente
2. Verifique se os arquivos `assets/snake-dark.svg` e `assets/snake-light.svg` foram gerados
3. Confirme que os caminhos no README estão corretos

## Banner não aparece

**Causa**: Caminho do arquivo `assets/banner.svg` incorreto ou arquivo corrompido.

**Solução**:
1. Verifique se o arquivo `assets/banner.svg` existe no repositório
2. Confirme se o caminho no README está correto
