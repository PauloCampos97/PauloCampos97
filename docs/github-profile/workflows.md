# Workflows

## metrics.yml

Gera **2 SVGs** com métricas do perfil GitHub, divididos em dois jobs independentes.

**Trigger**: Agendado diariamente (00:00 UTC), push na main, ou manual (workflow_dispatch).

### Job: overview

Gera `metrics/overview.svg` com visão geral do perfil.

**Plugins utilizados**:
- Base: header, activity, community, repositories, metadata
- Languages: principais linguagens com percentuais
- Isocalendar: calendário de contribuições (semestral)

### Job: extras

Gera `metrics/extras.svg` com métricas complementares.

**Plugins utilizados**:
- Achievements: conquistas do GitHub (formato compacto)
- Follow-up: estatísticas de issues e PRs
- Lines: linhas de código alteradas
- Notable: contribuições notáveis em organizações

**Secrets necessários**: `METRICS_TOKEN`

---

## snake.yml

Gera a animação snake a partir da grade de contribuições do GitHub.

**Trigger**: Agendado diariamente (00:00 UTC), push na main, ou manual (workflow_dispatch).

### Job: snake

- Usa `Platane/snk/svg-only@v3` para gerar os SVGs
- Gera 2 arquivos: `assets/snake-dark.svg` (tema escuro) e `assets/snake-light.svg` (tema claro)
- Faz commit automático dos SVGs atualizados via `stefanzweifel/git-auto-commit-action@v5`

**Secrets necessários**: Nenhum (usa apenas `github_user_name`).

---

## Notas

- Ambos os workflows possuem `concurrency` configurado para cancelar execuções duplicadas automaticamente.
- O workflow `metrics.yml` executa em ~30 segundos por job.
- O workflow `snake.yml` executa em ~15 segundos.
