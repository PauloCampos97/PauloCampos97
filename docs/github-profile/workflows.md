# Workflows

## metrics.yml

Gera 1 SVG com visão geral do perfil.

**Trigger**: Agendado diariamente (00:00 UTC), push na main, ou manual.

**Plugins utilizados**:
- Base (overview): header, activity, community, repositories, metadata

**Secrets necessários**: `METRICS_TOKEN`

## Notas

- Apenas 1 workflow é mantido para simplicidade e performance
- O workflow é executado em ~30 segundos (redução de ~90% vs. configuração anterior com múltiplos plugins)
