# 🤖 IA Study Map: Orquestrador de Carreira

> **Transforme sua trajetória profissional com planos de estudo gerados por um sistema de Agentes de IA especializados.**

Este repositório contém uma metodologia de **Multi-Agent Prompting** desenhada para criar roteiros de estudo hiper-personalizados. O projeto resolve o problema de cronogramas genéricos ao dividir a inteligência em duas etapas distintas: **Diagnóstico de Perfil** e **Arquitetura de Aprendizado**.

---

## 🏗️ Arquitetura do Sistema

O fluxo de trabalho foi estruturado para garantir que o plano de estudos seja tecnicamente denso, mas realisticamente adaptado à rotina do usuário.

### 🕵️ Agente 1: O Analista de Perfil (Profile Intelligence)
**Função:** Coleta, Entrevista e Contextualização.
- **Objetivo:** Mapear o "quem", o "onde" e o "quanto".
- **Ação:** Através de um prompt estruturado, a IA interage com o usuário para extrair:
    - Experiência prévia e nível técnico atual.
    - Objetivo de carreira (ex: Transição para Dados, Especialização em Cloud).
    - **Disponibilidade real:** Horas por dia e dias por semana.
- **Output:** Um *Profile Briefing* padronizado que serve de combustível para o Agente 2.

### 📅 Agente 2: O Arquiteto de Aprendizado (Curator & Scheduler)
**Função:** Estruturação, Curadoria e Cronograma.
- **Objetivo:** Transformar o briefing em um plano de ação executável.
- **Lógica:** Utiliza os dados do Agente 1 para definir a granularidade do conteúdo. Se o Agente 1 identifica "1h por dia", o Agente 2 quebra os módulos em pílulas de conhecimento curtas e diretas.
- **Output:** Um cronograma detalhado com marcos de sucesso (Milestones) e sugestões de temas baseados na stack escolhida.

---

## 🚀 Como Utilizar

1. **Executar o Agente 1:** 
   Copie o conteúdo de `/prompts/agent-1-analyst.md` e cole na sua IA de preferência. Responda às perguntas até que ela gere o seu resumo de perfil.
   
2. **Executar o Agente 2:** 
   Copie o resumo gerado pelo Agente 1. Em seguida, utilize o prompt de `/prompts/agent-2-architect.md` colando o resumo no campo indicado.

3. **Resultado:** 
   Você terá um plano de estudos formatado em Markdown, pronto para ser seguido.

---

## 📂 Estrutura do Repositório

```bash
├── 📁 prompts/
│   ├── 📄 agent-1-analyst.md    # Engenharia de prompt para coleta de dados
│   └── 📄 agent-2-architect.md  # Prompt focado em output de cronograma
├── 📁 examples/
│   └── 📄 sample-output.md      # Exemplo de um plano gerado com sucesso
└── 📄 README.md                 # Documentação do projeto

## 🛠️ Tecnologias & Inspiração

- **Engenharia de Prompt:** Otimizado para GPT-4, Claude 3 e Gemini.
- **Metodologia:** Inspirado no ecossistema de aprendizado da **DIO (Digital Innovation One)**.
- **Formatação:** Todo o output é gerado em Markdown para fácil integração com Notion ou Obsidian.

---

## 🤝 Contribuindo

Caso encontre uma forma de tornar os agentes mais precisos:

1.  Faça um **Fork**.
2.  Crie uma branch (`git checkout -b feature/melhoria-agente`).
3.  Faça um **Commit** (`git commit -m 'Melhoria na lógica de coleta do Agente 1'`).
4.  Faça um **Push** e abra um **Pull Request**.

---

⭐ **Dica:** A qualidade do seu plano depende da honestidade das informações fornecidas ao Agente 1!
