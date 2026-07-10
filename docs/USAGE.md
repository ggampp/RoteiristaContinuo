# Como Usar a Skill RoteiristaContinuo

## 1. Importando no Claude

1. Acesse o Claude (claude.ai ou app desktop)
2. Vá em **Skills** (no menu lateral)
3. Clique em **Import Skill**
4. Selecione o arquivo `SKILL.md` deste repositório
5. A skill aparecerá como "RoteiristaContinuo"

## 2. Usando em Agentes Programáticos

### LangGraph / CrewAI

```python
# Exemplo básico
system_prompt = open("SKILL.md").read()

# Depois use no seu agente normalmente
```

### MCP (Model Context Protocol)

A skill é compatível com MCP. Você pode carregar o conteúdo do `SKILL.md` como uma ferramenta ou instrução de sistema no seu servidor MCP.

## 3. Prompt de Ativação Recomendado

```
Ative a skill RoteiristaContinuo.

Quero criar um [trailer / esquete] sobre: [sua ideia aqui]
Duração desejada: [ex: 45 segundos]
Estilo visual: [ex: cinematográfico realista, anime, cyberpunk]
Plataforma alvo: [ex: YouTube, Instagram Reels, TikTok]
Tom: [ex: misterioso, humorístico, épico, emocional]
```

## 4. Fluxo Esperado da Skill

A skill sempre seguirá este fluxo:

1. **Clarificar** o pedido (se necessário)
2. **Criar Bible de Personagens e Estilo Visual** (obrigatório)
3. **Definir estrutura narrativa**
4. **Quebrar em planos** com referência constante à Bible
5. **Validar continuidade**
6. **Entregar** JSON + Markdown

## 5. Dicas de Uso Avançado

- Combine com **PenShot** para gerar prompts de vídeo a partir do JSON gerado.
- Use com **ArcReel** ou **Toonflow** para pipeline completo de vídeo.
- Peça à skill para gerar múltiplas versões do mesmo conceito (A/B testing de ganchos).

## 6. Exemplo de Saída

A skill sempre retorna:
- Uma seção clara de **Bible de Personagens e Estilo Visual**
- Lista de planos com prompts visuais prontos para IA de vídeo
- Versão JSON estruturada para automação