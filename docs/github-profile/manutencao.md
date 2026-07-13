# Manutenção

## Atualização dos workflows

Os workflows são executados automaticamente via cron:
- `metrics.yml`: 00:00 UTC diariamente (inclui métricas gerais + WakaTime)
- `snake.yml`: 00:00 UTC diariamente

Para executar manualmente:
1. Acesse **Actions** no GitHub
2. Selecione o workflow desejado
3. Clique em **Run workflow**

## Verificação de saúde (recomendado: mensal)

1. Acesse **Actions** e verifique se há falhas recorrentes
2. Verifique se os SVGs estão sendo gerados corretamente
3. Confirme se o token `METRICS_TOKEN` não expirou
4. Valide se os links do README continuam funcionando
5. Verifique se a branch `output` existe para a snake animation

## Renovação de tokens

- **METRICS_TOKEN**: Se configurado com expiração, renove antes do vencimento
- **WAKATIME_API_KEY**: Não expira, mas pode ser revogada manualmente

## Limpeza

Os workflows são configurados com `concurrency` para cancelar execuções duplicadas automaticamente.
