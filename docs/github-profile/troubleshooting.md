# Troubleshooting

## Workflow falha com "Resource not accessible by integration"

**Causa**: Permissões insuficientes do GITHUB_TOKEN.

**Solução**: Vá em Settings → Actions → General → Workflow permissions → "Read and write permissions"

## Workflow falha com "Bad credentials"

**Causa**: Token expirado ou inválido.

**Solução**: Renove o `METRICS_TOKEN` em Settings → Developer settings → Personal access tokens.

## WakaTime não mostra dados

**Causa**: API key incorreta ou sem dados registrados.

**Solução**:
1. Verifique se a extensão WakaTime está instalada e configurada no VS Code
2. Confirme o valor do secret `WAKATIME_API_KEY`
3. Teste a chave em [wakatime.com/api-key](https://wakatime.com/api-key)

## SVGs não são atualizados

**Causa**: Workflow não executou ou falhou.

**Solução**: Vá em **Actions**, selecione o workflow e execute manualmente.

## Snake animation não aparece

**Causa**: Branch `output` não foi criada.

**Solução**: Execute o workflow `snake.yml` manualmente. A branch será criada automaticamente.
