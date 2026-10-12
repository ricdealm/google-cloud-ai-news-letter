## 🚀 Gemini Enterprise Agent Platform

### 🧠 Modelos de IA

| Funcionalidade / Atualização | Detalhes | Link de Documentação Pública |
| :--- | :--- | :--- |
| **TabFM (Lançamento)** | Modelo fundacional zero-shot focado especificamente na classificação e regressão de dados tabulares (tabelas). Ao tratar predições estruturadas como aprendizado em contexto (ICL), ele elimina a necessidade de treinar modelos do zero (como XGBoost), otimizar hiperparâmetros ou fazer engenharia de atributos manual. Será integrado ao BigQuery em breve via comando SQL AI.PREDICT. | [Blog do Google Research – TabFM](https://research.google/blog/introducing-tabfm-a-zero-shot-foundation-model-for-tabular-data/) |
| **Claude Sonnet 5 (GA)** | O novo modelo de médio porte da Anthropic está disponível no Model Garden. Traz excelente equilíbrio entre custo e raciocínio avançado para fluxos de codificação e multiagentes.<br><br>Este modelo estará com preço de tokens reduzido até 31 de Agosto de 2026, U$2 por milhão de tokens de input e U$10 por milhão de tokens de output. Em 1 de Setembro, o preço de lista normal do modelo passa a ser U$3 por milhão de tokens de input e U$15 por milhão de tokens de output. | [Claude no Model Garden](https://cloud.google.com/products/model-garden/claude)<br>[Model Card](https://docs.cloud.google.com/gemini-enterprise-agent-platform/models/partner-models/claude/sonnet-5) |
| **Public Preview - Gemini Distillation Service** | O Gemini Distillation Service (Destilação) permite que os usuários treinem um modelo "aluno" menor e mais eficiente, utilizando as saídas e os padrões de raciocínio de um modelo "professor" maior e mais capaz. Embora os modelos de fronteira representem o estado da arte em IA, eles podem ser superdimensionados para casos de uso corporativos específicos. A destilação preenche essa lacuna, possibilitando eficiência de nível de produção (menor latência e custo) e permitindo, ao mesmo tempo, que modelos menores alcancem um nível de raciocínio mais profundo.<br><br>Ao contrário do ajuste fino supervisionado (SFT) padrão, que utiliza apenas a saída de texto final, a destilação aproveita:<br>- Respostas do professor: A saída textual final.<br>- Pensamentos brutos: Os caminhos de raciocínio internos gerados pelo modelo professor.<br>Modelos suportados: Modelo professor: `gemini-3.1-pro` / Modelo aluno: `gemini-2.5-flash`. | [Gemini Distillation Service](https://docs.cloud.google.com/gemini-enterprise-agent-platform/models/tuning/distillation) |
| **Public Preview - Reinforcement Learning Fine-tuning on Gemini** | Lançamento da prévia pública do ajuste fino via Aprendizado por Reforço (Reinforcement Learning) para o Gemini. O Aprendizado por Reforço (RL) é uma técnica poderosa para adaptar LLMs de modo a maximizar a recompensa de feedback fornecida por uma função de recompensa definida pelo usuário. O modelo explora diversas respostas possíveis, observa uma recompensa numérica para cada uma e ajusta gradualmente seu comportamento para que as respostas de alta recompensa se tornem mais prováveis.<br><br>Essa técnica é excelente em cenários que exigem raciocínio em múltiplas etapas, tomada de decisão complexa ou a compreensão de nuances sutis nos prompts. Permite aos usuários aprimorar a capacidade de raciocínio e a qualidade das respostas dos modelos Gemini para fluxos agênticos específicos. | [Reinforcement Learning Fine-tuning on Gemini](https://docs.cloud.google.com/gemini-enterprise-agent-platform/models/tuning/reinforcement-tuning) |
| **GA - Multimodal Supervised Fine-tuning for Gemini models** | Novidades:<br>- **Part-Level Media File Resolution:** Controle da resolução com granularidade individual por parte, permitindo resoluções mistas para a modalidade de imagem.<br>- **Default Function Call Tuning:** Ajuste de chamadas de função suportado nativamente, permitindo que os modelos aprendam interações de API estruturadas.<br>- **Multimodal Inputs & Text-Only Outputs:** Suporte a texto, imagem, PDF, vídeo, áudio e function calling.<br>- **Multi-Region Serving:** Modelos ajustados (Tuned) e endpoints disponíveis em múltiplas regiões dos EUA e UE. | [Multimodal Supervised Fine-tuning](https://docs.cloud.google.com/gemini-enterprise-agent-platform/models/tuning/supervised-tuning) |
| **Open Knowledge Format (Artigo Técnico)** | Apresentação do Open Knowledge Format (OKF), uma especificação aberta que formaliza o padrão LLM-wiki em um formato portátil e interoperável. Trata-se de um padrão neutro em relação a fornecedores, adequado tanto para agentes quanto para humanos, para representar metadados, contexto e o conhecimento curado corporativo. | [Open Knowledge Format](https://cloud.google.com/blog/products/data-analytics/how-the-open-knowledge-format-can-improve-data-sharing?e=48754805) |

---

### 🛠️ Infraestrutura e Plataforma de Agentes (Agent Platform)

| Funcionalidade / Atualização | Detalhes | Link de Documentação Pública |
| :--- | :--- | :--- |
| **Agent Gateway (GA)** | Componente de rede que protege, centraliza e governa a conectividade nas interações usuário-agente, agente-ferramenta e entre múltiplos agentes. | [Agent Gateway](https://docs.cloud.google.com/gemini-enterprise-agent-platform/govern/gateways/agent-gateway-overview?hl=pt-br) |
| **Agent Observability (GA)** | Monitoramento de performance e rastreamento nativo (*tracing* via OpenTelemetry habilitado por padrão) para agentes de IA e servidores MCP corporativos. | [Agent Observability (GA)](https://docs.cloud.google.com/stackdriver/docs/observability/agent-observability) |
| **Agent Registry (GA)** | Catálogo corporativo unificado para descobrir e registrar agentes e servidores MCP. Traz suporte oficial à API v1, bibliotecas de cliente e gerenciamento via Terraform. | [Agent Registry (GA)](https://docs.cloud.google.com/agent-registry/overview) |
| **Agent Identity API (Preview)** | Nova API (`agentidentity.googleapis.com`) para gerenciar identidades de agentes (SPIFFE ID), substituindo a antiga API IAM Connectors com segurança aprimorada. | [Agent Identity API (Preview)](https://docs.cloud.google.com/iam/docs/agent-identity-overview) |
| **Memory Bank & Sessions MREP (GA)** | Endpoints globais e multirregionais para armazenamento e isolamento seguro de sessões de chat e memórias de agentes de IA corporativos. | [Memory Bank](https://docs.cloud.google.com/gemini-enterprise-agent-platform/scale/memory-bank)<br>[MREP](https://docs.cloud.google.com/gemini-enterprise-agent-platform/scale/memory-bank/setup#multi-regional-global-endpoints) |

---

### 🛡️ Segurança e Governança de IA

| Funcionalidade / Atualização | Detalhes | Link de Documentação Pública |
| :--- | :--- | :--- |
| **Semantic Governance Policies (Preview)** | Camada de segurança inteligente que avalia as ferramentas que o agente quer chamar em tempo real, validando-as contra restrições em linguagem natural (NLC) e intenções autorizadas. | [Semantic Governance](https://docs.cloud.google.com/gemini-enterprise-agent-platform/govern/policies/semantic-governance-overview) |
| **Model Armor para Agent Gateway (GA)** | Permite que administradores ativem o Model Armor no gateway de rede para aplicar filtros automáticos de segurança e toxicidade sobre tudo o que entra e sai do agente. | [Model Armor para Agent Gateway](https://docs.cloud.google.com/model-armor/model-armor-agent-gateway-integration) |
| **Painel de Descobertas de Segurança** | Monitoramento de vulnerabilidades em runtimes de agentes (como Cloud Run) e gráficos históricos de tendências de violação de conteúdo direto no console. | [Painel de Descobertas de Segurança](https://docs.cloud.google.com/security-command-center/docs/review-ai-security) |
| **Abuso e Zero Data Retention (ZDR)** | Documentação oficial atualizada conforme as regras de segurança do *Advanced AI Safety Addendum*, cobrindo novas diretrizes para o Claude Mythos e Claude Opus. | [Abuso e Zero Data Retention (ZDR)](https://docs.cloud.google.com/gemini-enterprise-agent-platform/models/abuse-monitoring) |

---

## 📱 Gemini Enterprise App – Novidades de Junho / Julho

### 💬 Integrações e Acessibilidade

| Funcionalidade / Atualização | Detalhes | Link de Documentação Pública |
| :--- | :--- | :--- |
| **Geração em Canvas (Public Preview)** | Área lateral interativa que permite editar, visualizar e refinar documentos de texto ou slides lado a lado com o chat antes de exportar para GDocs, GSlides ou PDF. | [Canvas no Gemini Enterprise](https://docs.cloud.google.com/gemini/enterprise/docs/assistant-canvas)<br>[Gerenciar Recursos Web](https://docs.cloud.google.com/gemini/enterprise/docs/manage-web-app-features) |
| **Gemini Mobile App (GA)** | Aplicativo para Android e iOS agora Generally Available para usuários que utilizam o Google Identity, com login rápido por QR Code. | [Configurar Mobile App](https://docs.cloud.google.com/gemini/enterprise/docs/configure-mobile-app)<br>[Usar Mobile App](https://docs.cloud.google.com/gemini/enterprise/docs/use-the-mobile-app) |
| **Integração Nativa com Slack (GA)** | Conversa direta com o Gemini Enterprise por mensagens diretas (DMs) ou comandos / dentro do próprio ambiente de trabalho do Slack. | [Configurar App para Slack](https://docs.cloud.google.com/gemini/enterprise/docs/configure-slack-app) |
| **Workflow Agents (GA com Allowlist)** | Capacidade de criar, importar, atualizar e usar agentes de fluxo de trabalho no aplicativo da web do Gemini Enterprise, automatizando sequências de etapas combinando IA e intervenção humana. | [Release Notes do Gemini Enterprise (18/06/2026)](https://docs.cloud.google.com/gemini/enterprise/docs/release-notes#June_18_2026) |
| **Habilidades Personalizadas / Skills (GA com Allowlist)** | Criação e gestão de habilidades reutilizáveis no aplicativo web para direcionar tarefas corporativas padronizadas. | [Release Notes do Gemini Enterprise (17/06/2026)](https://docs.cloud.google.com/gemini/enterprise/docs/release-notes#June_17_2026) |

---

### ⚙️ Gestão de IA e Modelos

| Funcionalidade / Atualização | Detalhes | Link de Documentação Pública |
| :--- | :--- | :--- |
| **Observabilidade de Deep Research (Preview)** | Administradores ganharam a capacidade de habilitar e acompanhar métricas de performance e logs de tracing individualmente para os agentes de Deep Research. | [Gerenciar Configurações de Observabilidade](https://docs.cloud.google.com/gemini/enterprise/docs/manage-observability-settings) |
| **Frameworks de Migração Assistida** | Guias e códigos abertos para facilitar a transição de plataformas de terceiros para o ambiente do Gemini Enterprise. | [Gemini Enterprise Migration Agent](https://github.com/GoogleCloudPlatform/generative-ai/tree/main/search/gemini-enterprise/ge-migration-agent) |
