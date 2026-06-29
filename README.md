# AI Template

Template para projetos de desenvolvimento de software assistido por IA usando [opencode](https://opencode.ai).

## Estrutura

```
├── .opencode/          # Configuração do opencode
│   ├── commands/       # Comandos personalizados (ex: opsx-explore)
│   ├── skills/         # Skills instaladas
│   └── package.json    # Dependências do opencode
├── openspec/           # OpenSpec — framework de desenvolvimento spec-driven
│   └── config.yaml     # Configuração do OpenSpec
├── SKILLS.md           # Lista de skills disponíveis
└── README.md
```

## Skills Instaladas

| Skill | Descrição |
|-------|-----------|
| **coding-guidelines** | Diretrizes para reduzir erros comuns de codificação em LLMs |
| **context7** | Busca documentação atualizada de bibliotecas e frameworks |
| **docs-writer** | Escrita e revisão de documentação |
| **domain-analysis** | Mapeamento de domínios com DDD Strategic Design |
| **excalidraw-studio** | Geração de diagramas Excalidraw |
| **graphify** | Criação de grafos de conhecimento a partir de código/docs |
| **mermaid-studio** | Diagramas Mermaid (SVG/PNG/ASCII) |
| **skill-architect** | Criação de novas skills |
| **spec-driven-eval** | Avaliação de implementação contra PRD/spec |
| **tactical-ddd** | Refatoração para modelos ricos com DDD tático |
| **technical-design-doc-creator** | Criação de Documentos de Design Técnico |
| **tlc-spec-driven** | Planejamento em 4 fases: Spec → Design → Tasks → Execute |

## OpenSpec

O diretório `openspec/` contém a configuração do framework **OpenSpec**, que permite:

- **Propostas** — Definição de escopo e objetivos
- **Designs** — Decisões técnicas e arquiteturais
- **Tasks** — Divisão de trabalho em tarefas atômicas
- **Specs** — Especificações detalhadas de funcionalidades

## Comandos

| Comando | Descrição |
|---------|-----------|
| `/opsx-explore` | Modo exploratório para pensar, investigar e esclarecer requisitos sem implementar |

## Uso

1. Ative uma skill relevante para sua tarefa (ex: `tlc-spec-driven` para planejamento)
2. Use o OpenSpec para capturar requisitos e decisões
3. Implemente com verificação atômica por tarefa
