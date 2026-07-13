# Manutenção

## Atualização do workflow

O workflow é executado automaticamente via cron:
- `metrics.yml`: 00:00 UTC diariamente

Para executar manualmente:
1. Acesse **Actions** no GitHub
2. Selecione o workflow desejado
3. Clique em **Run workflow**

## Verificação de saúde (recomendado: mensal)

1. Acesse **Actions** e verifique se há falhas recorrentes
2. Verifique se o SVG foi gerado corretamente
3. Confirme se o token `METRICS_TOKEN` não expirou
4. Valide se os links do README continuam funcionando

## Renovação de tokens

- **METRICS_TOKEN**: Se configurado com expiração, renove antes do vencimento

## Limpeza

O workflow é configurado com `concurrency` para cancelar execuções duplicadas automaticamente.
