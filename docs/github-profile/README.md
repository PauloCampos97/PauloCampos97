# GitHub Profile — Documentação

Bem-vindo à documentação do perfil GitHub de [PauloCampos97](https://github.com/PauloCampos97).

Este repositório mantém um perfil profissional automatizado com métricas dinâmicas, animações e deploy contínuo via GitHub Actions.

## Índice

- [Instalação](instalacao.md)
- [Tokens e Secrets](tokens.md)
- [Workflows](workflows.md)
- [Manutenção](manutencao.md)
- [Troubleshooting](troubleshooting.md)
- [Upgrade](upgrade.md)

## Visão Geral

O perfil é composto pelos seguintes blocos, organizados de cima para baixo:

| Seção | Descrição |
|---|---|
| **Banner SVG** | Banner visual com gradiente e tags de especialização |
| **Nome + Cargo** | Nome e título profissional estilizados |
| **Sobre Profissional** | Parágrafo com descrição da atuação e filosofia de trabalho |
| **Stack Principal** | 6 categorias de tecnologias (Frontend, Backend, Database, Cloud, DevOps, Ferramentas) |
| **GitHub Analytics** | 2 SVGs de métricas (overview + extras) gerados pelo lowlighter/metrics |
| **Snake de Contribuições** | Animação SVG da grade de contribuições (dark/light mode) |
| **Projetos em Destaque** | Cards com border-radius e badge "Destaque" |
| **Atualmente Estudando** | Tecnologias em aprendizado com descrição |
| **Contato** | LinkedIn, Email e Instagram com badges estilizados |
| **Footer** | Badges de status (última atualização, status dos workflows) |

## Workflows

O repositório possui **2 workflows** de GitHub Actions:

| Workflow | Arquivo | Job | Gera |
|---|---|---|---|
| GitHub Metrics | `metrics.yml` | `overview` | `metrics/overview.svg` |
| GitHub Metrics | `metrics.yml` | `extras` | `metrics/extras.svg` |
| Generate Snake | `snake.yml` | `snake` | `assets/snake-dark.svg`, `assets/snake-light.svg` |

## Tecnologias

| Ferramenta | Versão | Função |
|---|---|---|
| lowlighter/metrics | latest | Geração dos SVGs de métricas do GitHub |
| Platane/snk | v3 | Geração da animação snake de contribuições |
| stefanzweifel/git-auto-commit-action | v5 | Commit automático dos artefatos gerados |

## Cores do Projeto

```yaml
primary:   "#bf3b48"  # Vermelho Alpar
secondary: "#152039"  # Azul escuro Alpar
```

## Estrutura de Arquivos

```
.
├── .github/
│   └── workflows/
│       ├── metrics.yml          # Geração de métricas (overview + extras)
│       └── snake.yml            # Geração da snake de contribuições
├── assets/
│   ├── banner.svg               # Banner visual do perfil
│   ├── snake-dark.svg           # Snake modo escuro
│   └── snake-light.svg          # Snake modo claro
├── metrics/
│   ├── overview.svg             # Métricas principais
│   └── extras.svg               # Métricas extras (achievements, linhas, etc.)
├── docs/
│   └── github-profile/          # Documentação do perfil
└── README.md                    # Perfil principal
```
