# Manutenção

## Atualização dos workflows

Os workflows são executados automaticamente via cron:

- `metrics.yml`: 00:00 UTC diariamente (2 jobs: overview e extras)
- `snake.yml`: 00:00 UTC diariamente

Para executar manualmente:
1. Acesse **Actions** no GitHub
2. Selecione o workflow desejado (GitHub Metrics ou Generate Snake)
3. Clique em **Run workflow**

## Verificação de saúde (recomendado: mensal)

1. Acesse **Actions** e verifique se há falhas recorrentes em ambos os workflows
2. Verifique se os SVGs foram gerados corretamente:
   - `metrics/overview.svg`
   - `metrics/extras.svg`
   - `assets/snake-dark.svg`
   - `assets/snake-light.svg`
3. Confirme se o token `METRICS_TOKEN` não expirou
4. Valide se os links do README continuam funcionando
5. Verifique se o banner `assets/banner.svg` está sendo exibido corretamente

## Renovação de tokens

- **METRICS_TOKEN**: Se configurado com expiração, renove antes do vencimento

## Limpeza

Ambos os workflows são configurados com `concurrency` para cancelar execuções duplicadas automaticamente.
