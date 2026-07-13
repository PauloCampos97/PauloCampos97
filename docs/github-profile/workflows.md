# Workflows

## metrics.yml

Gera 8 SVGs com métricas do perfil.

**Trigger**: Agendado diariamente (00:00 UTC), push na main, ou manual.

**Plugins utilizados**:
- Base (general): header, activity, community, repositories, metadata
- Languages: top linguagens com detalhes
- Achievements: conquistas do GitHub
- Skyline: calendário 3D de contribuições
- Habits: hábitos de codificação
- Calendar: calendário de commits
- Repositories: repositórios em destaque
- WakaTime: estatísticas WakaTime

**Secrets necessários**: `METRICS_TOKEN`, `WAKATIME_API_KEY`

## snake.yml

Gera a animação da cobrinha no grid de contribuições.

**Trigger**: Agendado diariamente (00:00 UTC), push na main, ou manual.

**Versão**: Platane/snk@v3

**Formatos gerados**:
- `github-contribution-grid-snake.svg` (modo claro)
- `github-contribution-grid-snake-dark.svg` (modo escuro)

**Deploy**: Publicado na branch `output/snake/`

## wakatime.yml

Workflow dedicado exclusivamente às métricas WakaTime.

**Trigger**: Agendado diariamente (06:00 UTC) ou manual.
