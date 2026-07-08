# AI Template

Template para projetos de desenvolvimento de software assistido por IA usando [opencode](https://opencode.ai).

## Estrutura

```
├── .opencode/          # Configuração do opencode
│   ├── commands/       # Comandos personalizados (ex: explore)
│   ├── skills/         # Skills instaladas
│   └── package.json    # Dependências do opencode
├── SKILLS.md           # Lista de skills disponíveis
└── README.md
```

## Skills Instaladas

| Skill | Descrição |
|-------|-----------|
| **context7** | Busca documentação atualizada de bibliotecas e frameworks |
| **docs-writer** | Escrita e revisão de documentação |
| **domain-analysis** | Mapeamento de domínios com DDD Strategic Design |
| **excalidraw-studio** | Geração de diagramas Excalidraw |
| **graphify** | Criação de grafos de conhecimento a partir de código/docs |
| **mermaid-studio** | Diagramas Mermaid (SVG/PNG/ASCII) |
| **skill-architect** | Criação de novas skills |
| **spec-driven-eval** | Avaliação de implementação contra PRD/spec |
| **technical-design-doc-creator** | Criação de Documentos de Design Técnico |
| **code-review-skill** | Revisão de código estruturada para 20+ linguagens/frameworks |
| **tlc-spec-driven** | Planejamento em 4 fases: Spec → Design → Tasks → Execute |
| **modular-architecture** | Arquitetura modular com bounded contexts, facades e 10 princípios de design |

## Comandos

| Comando | Descrição |
|---------|-----------|
| `/explore` | Modo exploratório para pensar, investigar e esclarecer requisitos sem implementar |
| `/tdd` | Cria um Documento de Design Técnico (TDD) para um projeto e salva em `specs/tdd.md` |
| `/prd` | Cria um Product Requirements Document (PRD) para um projeto e salva em `specs/prd.md` |
| `/roadmap` | Gera roadmap com features e tarefas a partir de `specs/tdd.md` e `specs/prd.md` |
| `/plan` | Gera plano de implementação a partir de `specs/prd.md` e `specs/roadmap.md` |
| `/generate` | Executa o plano de implementação e gera código em `src/` a partir de `specs/plan.md` |
| `/review` | Revisa o código em `src/` comparando com `specs/prd.md` e `specs/plan.md` |

## Uso

1. Ative uma skill relevante para sua tarefa (ex: `tlc-spec-driven` para planejamento)
2. Implemente com verificação atômica por tarefa
