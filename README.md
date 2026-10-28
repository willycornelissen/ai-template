# AI Template

Template para projetos de desenvolvimento de software assistido por IA usando [opencode](https://opencode.ai).

## Estrutura

```
├── .agents/            # Skills do Reversa (Engenharia Reversa)
├── .opencode/          # Configuração do opencode
│   ├── commands/       # Comandos personalizados (ex: explore)
│   ├── skills/         # Skills instaladas (Core e Frontend)
│   ├── docs/           # Documentação de padrões de código
│   └── package.json    # Dependências do opencode
├── AGENTS.md           # Diretrizes comportamentais para o agente de IA
├── FRONTEND.md         # Guia e documentação das skills de Frontend/Design
├── LEGADO.md           # Guia e documentação do Reversa (Engenharia Reversa)
└── SKILLS.md           # Lista completa de skills disponíveis
```

## Skills Instaladas

### Core Skills (`.opencode/skills/`)

| Skill | Descrição |
|-------|-----------|
| **code-review-skill** | Revisão de código estruturada para 20+ linguagens/frameworks |
| **context7** | Busca documentação atualizada de bibliotecas e frameworks |
| **docs-writer** | Escrita e revisão de documentação |
| **domain-analysis** | Mapeamento de domínios com DDD Strategic Design |
| **excalidraw-studio** | Geração de diagramas Excalidraw |
| **graphify** | Criação de grafos de conhecimento a partir de código/docs |
| **mermaid-studio** | Diagramas Mermaid (SVG/PNG/ASCII) |
| **modular-architecture** | Arquitetura modular com bounded contexts, facades e 10 princípios de design |
| **office-hours** | YC Office Hours: diagnóstico de produto para startups ou brainstorm para builders |
| **skill-architect** | Criação de novas skills |
| **spec-driven-eval** | Avaliação de implementação contra PRD/spec |
| **technical-design-doc-creator** | Criação de Documentos de Design Técnico |
| **tlc-discover** | Entrevista de ideias não refinadas gerando veredito e documento de design |
| **tlc-implement** | Implementação com checks congelados, provas e verificação independente |
| **tlc-plan** | Planejamento acionável a partir de requisições/PRDs com critérios EARS |
| **tlc-prd** | Entrevista de produto e geração de PRD completo |
| **tlc-spec-driven** | Planejamento em 4 fases: Spec → Design → Tasks → Execute |
| **tlc-spec-lean** | Spec-driven com obrigações congeladas, checks com provas e verificação |

### Frontend & Design Skills (`.opencode/skills/`)

Documentação completa em [FRONTEND.md](FRONTEND.md).

| Skill | Descrição |
|-------|-----------|
| **ui-ux-pro-max** | Inteligência de design UI/UX para web e mobile (estilos, paletas, fontes, UX, GSAP, gráficos) |
| **design** | Design abrangente: logo (Gemini AI), identidade corporativa (CIP), ícones, apresentações, banners |
| **ui-styling** | Interfaces com shadcn/ui (Radix + Tailwind), componentes acessíveis e visual canvas |
| **design-system** | Arquitetura de tokens em 3 camadas, variáveis CSS, escalas e geração de slides |
| **brand** | Identidade de marca: voz, guias visuais, gestão de ativos e sync com tokens |
| **banner-design** | Banners multi-formato para redes sociais, anúncios, hero e impressão (22 estilos) |
| **ai-artist** | Geração de imagens Nano Banana / Gemini com 129 prompts curados e 3 modos |
| **ai-multimodal** | Processamento e geração de mídia via Gemini API (áudio, imagem, vídeo, PDF) |
| **chrome-devtools** | Automação de browser e renderização visual com Puppeteer via CLI |
| **frontend-design** | Interfaces frontend de alta qualidade em HTML/CSS |
| **assets-organizing** | Convenções de organização de outputs em `assets/` por tópico, data e slug |
| **slides** | Apresentações HTML estratégicas com Chart.js, design tokens e copywriting |

### Engenharia Reversa — Reversa Skills (`.agents/skills/`)

Documentação completa em [LEGADO.md](LEGADO.md).

O **Reversa** é um framework de engenharia reversa para descobrir, documentar e especificar sistemas legados em artefatos executáveis.

| Skill | Descrição |
|-------|-----------|
| **reversa** | Ponto de entrada principal para análise completa de sistemas legados |
| **reversa-scout** / **reversa-archaeologist** / **reversa-architect** | Mapeamento de superfície, escavação de código e síntese arquitetural |
| **reversa-data-master** / **reversa-visor** / **reversa-detective** | Documentação de banco de dados, interfaces (screenshots) e regras de negócio |
| **reversa-writer** / **reversa-reviewer** | Geração de especificações executáveis (SDD) e revisão crítica |
| **reversa-forward** / **reversa-new** / **reversa-migrate** | Orquestradores do ciclo de evolução forward, projetos greenfield e migração de sistemas |
| **reversa-docs** / **reversa-arquitetura-3d** / **reversa-especialista-d3** | Geração de mini-site visual interativo, Code City 3D (Three.js) e mapas 2D (D3.js) |
| **reversa-refactor** / **reversa-debugger** / **reversa-debugger-fix** | Inventário de refatoração por ROI, registro de bugs e fluxo de correção com testes |

## Comandos

| Comando | Descrição |
|---------|-----------|
| `/doc` | Gera documentação do projeto e código em `documentation/` |
| `/generate` | Executa o plano de implementação e gera código em `src/` a partir de `specification/plan.md` |
| `/new-feature` | Cria uma nova funcionalidade completa: TDD, PRD, roadmap, plano, código, review e documentação. Uso: `/new-feature <slug>: <nome-da-feature>` |
| `/plan` | Gera plano de implementação a partir de `specification/prd.md` e `specification/roadmap.md` |
| `/prd` | Cria um Product Requirements Document (PRD) para um projeto e salva em `specification/prd.md` |
| `/idea` | YC Office Hours — explora ideias, problemas ou conceitos de produto e salva a ideia bruta em `specification/idea.md` e o resumo em `specification/research.md` |
| `/review` | Revisa o código em `src/` comparando com `specification/prd.md` e `specification/plan.md` |
| `/roadmap` | Gera roadmap com features e tarefas a partir de `specification/tdd.md` e `specification/prd.md` |
| `/tdd` | Cria um Documento de Design Técnico (TDD) para um projeto e salva em `specification/tdd.md` |
