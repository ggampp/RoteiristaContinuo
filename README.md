# RoteiristaContinuo

**Skill open-source para agentes de IA** especializada em roteirizar **trailers** e **esquetes** com **continuidade visual e narrativa** de alto nível.

Uma skill projetada para transformar ideias em roteiros cinematográficos prontos para produção com modelos de vídeo IA (Veo, Seedance, Sora, Kling etc.), garantindo consistência de personagens, cenários e fluxo narrativo.

## 🚀 O que esta skill entrega

- Criação obrigatória de **Bible de Personagens e Estilo Visual**
- Validação rigorosa de continuidade entre todos os planos
- Output estruturado (JSON + Markdown) otimizado para pipelines de vídeo
- Foco em conteúdo curto (trailers, Reels, TikTok, esquetes de 15s a 3 minutos)
- Linguagem cinematográfica profissional

## 📁 Estrutura do Repositório

```
RoteiristaContinuo/
├── README.md
├── SKILL.md                 # A skill principal
├── docs/
│   ├── USAGE.md
│   └── EXAMPLES.md
└── references/             # Resumos e links dos projetos que inspiraram
```

## 🔧 Como usar a Skill

### 1. No Claude (Skills)
Importe o arquivo `SKILL.md` em Skills > Import Skill.

### 2. Em agentes (LangGraph, CrewAI, MCP, Odysseus/Colmeia)
Use como system prompt ou ferramenta especializada.

**Prompt de ativação sugerido:**
> "Ative a skill RoteiristaContinuo. Quero um trailer/esquete sobre [ideia]. Duração: [X] segundos. Estilo: [Y]. Plataforma: [Z]."

## 📚 Projetos que Inspiraram Esta Skill

Esta skill foi criada após extensa pesquisa nos melhores projetos open-source de 2025-2026 para produção de vídeo com agentes.

### Principais Referências

| Projeto | Descrição | Link | Destaque para Continuidade |
|---------|---------------|------|---------------------------|
| **ArcReel** | Workbench completo com multi-agentes (Skill + Subagent). Fluxo novel → roteiro → design de personagens → vídeo. | [github.com/ArcReel/ArcReel](https://github.com/ArcReel/ArcReel) | Excelente: imagens de referência de personagens + "Clue Tracking" para props/cenas |
| **PenShot** (neopen) | Agente LangGraph que quebra roteiros em prompts de vídeo consistentes. | [github.com/neopen/story-shot-agent](https://github.com/neopen/story-shot-agent) | Um dos melhores: multi-level memory + Chroma retrieval + suporte nativo a **MCP** |
| **OpenStory** | Script/ideia → multi-cena com consistência automática de personagens e locações. | [openstory.so](https://openstory.so) | Define personagens e estilo uma vez e mantém em todos os shots |
| **Shanyin-screenwriting-master** | .skill file pronta para importar em Claude/GPT focada em formatos curtos (1-3min e 5-10min). | [github.com/Shanyin-ai/shanyin-screenwriting-master](https://github.com/Shanyin-ai/shanyin-screenwriting-master) | Literal skill de roteirista com estrutura narrativa forte |
| **Toonflow-app** | One-stop tool para short-drama com 3 camadas de agents + memória persistente. | [github.com/HBAI-Ltd/Toonflow-app](https://github.com/HBAI-Ltd/Toonflow-app) | Agent memory + infinite canvas para produção contínua |
| **OpenDirector** | 9 agentes especializados (incluindo Script Agent) a partir de uma frase. | [github.com/seme-org/open-director](https://github.com/seme-org/open-director) | Boa orquestração multi-agente para víeos curtos |

Outros projetos relevantes: wind-comic, Coconah/AI-Short-Drama-Agent-Skill, Genra Video Creator.

## 🤝 Contribuição

Sinta-se à vontade para abrir issues e PRs com melhorias na skill, novos exemplos ou integrações com ferramentas de vídeo.

## 🙏 Créditos

Skill criada por Grok para Guilherme Pimentel (ggampp), inspirada nos projetos acima e nas melhores práticas de agentic video production.

---

**RoteiristaContinuo** — Continuidade não é opcional. É o diferencial.