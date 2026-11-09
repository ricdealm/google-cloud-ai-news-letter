# Google Cloud AI Newsletter & Base de Conhecimento

Repositório central de documentação técnica e boletins informativos periódicos sobre as atualizações, lançamentos e anúncios da stack de inteligência artificial do Google (Gemini Enterprise Agent Platform, Model Garden, Agent Development Kit - ADK, Gemini Enterprise App, Segurança & Governança e FinOps).

🔗 **Repositório Remoto no GitHub:** [https://github.com/ricdealm/google-cloud-ai-news-letter.git](https://github.com/ricdealm/google-cloud-ai-news-letter.git)

---

## 🏛️ Estrutura e Arquitetura do Repositório

O projeto foi estruturado para suportar publicação contínua em formato Markdown (pronto para exportação para Confluence, GitHub Wiki, Notion ou e-mails corporativos) aliado a um visualizador interativo em HTML/Tailwind com suporte a filtros dinâmicos e busca instantânea:

```
google-cloud-ai-news-letter/
├── novidades_google_ai_09-11-2026.md  # Edição de 09/11/2026 (02 a 09/nov/2026) - 19 itens (Mais recente)
├── novidades_google_ai_02-11-2026.md  # Edição de 02/11/2026 (26/out a 02/nov/2026) - 13 itens
├── novidades_google_ai_26-10-2026.md  # Edição de 26/10/2026 (20 a 26/out/2026) - 12 itens
├── novidades_google_ai_19-10-2026.md  # Edição de 19/10/2026 (13 a 19/out/2026) - 11 itens
├── novidades_google_ai_12-10-2026.md  # Edição de 12/10/2026 (05 a 12/out/2026) - 9 itens
├── novidades_google_ai_04_10_2026.md  # Edição de 04/10/2026 (22/set a 03/out/2026) - 15 itens
├── novidades_google_ai_22-09-2026.md  # Edição de 22/09/2026 (14 a 21/set/2026) - 14 itens
├── novidades_google_ai_13-09-2026.md  # Edição de 13/09/2026 (19/ago a 12/set/2026) - 21 itens
├── novidades_google_ai_18-08-2026.md  # Edição de 18/08/2026 (09 a 17/ago/2026) - 13 itens
├── novidades_google_ai_08-08-2026.md  # Edição de 08/08/2026 (02 a 08/ago/2026) - 15 itens
├── novidades_google_ai_01-08-2026.md  # Edição de 01/08/2026 (21 a 31/jul/2026) - 16 itens
├── novidades_google_ai_20-07-2026.md  # Edição de 20/07/2026 (02 a 20/jul/2026) - 11 itens
├── novidades_google_ai_01-07-2026.md  # Edição de 01/07/2026 (16 a 30/jun/2026) - 22 itens
├── wiki_preview.html                  # Visualizador interativo em layout Wiki com filtros por semana e categoria
└── Readme.md                          # Este documento (arquitetura, funcionalidades e histórico de edições)
```

---

## 📦 Acervo e Funcionalidades (`wiki_preview.html` & Edições `.md`)

1. **Cobertura Temporal por Semana (13 Edições Catalogadas):**
   - **Acervo Completo:** **191 lançamentos** documentados entre 01/07/2026 e 09/11/2026.
   - **Filtro Rápido no Topo e Dropdown (`wiki_preview.html`):** Seleção direta por semana e busca combinada.
   - **Sidebar com Navegação e Contadores:** Menu lateral esquerdo com links âncora e contagem individual de novidades por edição.

2. **Distribuição por Categorias Técnicas (191 lançamentos no acervo):**
   - 🧠 **Modelos de IA (58 lançamentos):** Gemini Omni 1.2 Flash (GA), Gemini 4 Carbon (Frontier Cyber & Reasoning), Gemini 4 Argon (GA, Long Decodes de 1M tokens na Interactions API e regiões DRZ), Gemini Robotics ER 2 (Preview), Gemini 3.8 Flash/Flash-Lite TTS (GA), Gemini 3.5 Transcribe (GA), AlphaGenome (`alphagenome-004` gRPC/HTTP/2 streaming GA), Modelos Ajustados Gemini 3.x em Endpoints Globais (GA), Modelos OpenAI Nativos (`GPT-6 Astra`, `GPT-6.1 Sol`, `GPT-6 Luna`), Claude Models (Anthropic Managed GA, Opus/Sonnet/Haiku 5.5), xAI Grok 4.7 (GA), DeepSeek-V4.1-Flash e Gemini Nano Banana 2.1.
   - 🛠️ **Plataforma de Agentes, Dados & Infra (56 lançamentos):** Interface dedicada do Memory Bank no Console, Throughput Provisionado para Modelos com SFT (GA), CodeMender v0.16.0 e v0.18.0, Benchmark Physical-Engineering's Last Exam (PLE), BigQuery AI (`AI.PARSE_DOCUMENT`, `AI.CHUNK_DOCUMENT`, `AI.AGG`, `AI.FORECAST` com TimesFM 3.0 e `.bigquery` no Pandas/BigFrames), Agentic Data Cloud (System of Action), Antigravity Plugin Marketplace, Computer Use (GA com HITL), Virtualização Aninhada no GKE Autopilot (`/dev/kvm`), K8s Bridge open source para GKE, Agent Development Kit (ADK), AlloyDB AI e Spanner Iceberg Catalog.
   - 🛡️ **Segurança & Governança (17 lançamentos):** Controle de Disponibilidade de Modelos por Política de Localização de Recursos (`Resource Location Policies`), Ambient Quality Agent (AQuA), Antigravity Enterprise Gateway (GA), Model Armor, Content Safety Guardrails, VPC Service Controls, Data Residency e Criptografia CMEK.
   - 📱 **Gemini Enterprise App & Conectores (47 lançamentos):** Conector Adobe (Public Preview), Conector Federado para Salesforce CRM (GA), Comutação de Equipes no Mobile App, Geração de Vídeo com Gemini Omni 1.2 Flash (GA), Gemini Notebook Enterprise Visual Refresh (GA), Parceria Estratégica ServiceNow Action Fabric, Workspace Connectors v2 (rMCP para Docs, Sheets e Slides), Conectividade VPC e Egress com IP Estático para Servidores MCP Customizados (GA), Data Cloud Connectors 1P (Preview), BigQuery Conversational Analytics (GA), Gemini for Customer Experience (CX Agent Studio) e Google Flow for Enterprise.
   - ⚙️ **FinOps & Gestão de Modelos (13 lançamentos):** Créditos Pré-Pagos para Pay-as-you-go e Excedentes (GA), Cronograma de Transição de Licenças do Gemini Code Assist (até março/2027), Previsão Orçamentária e Hard Spend Caps no Gemini Enterprise App, Descontinuação do Gemini 3.6 Flash, Limites de Cota por Usuário Único (GA), Priority PayGo para Nano Banana 2.1 e Provisioned Throughput sem ramp limits.

3. **Busca Textual em Tempo Real:**
   - Pesquisa instantânea inteligente por nome de modelo, tecnologia, autoroute, tag de estágio (GA, Preview, Open Source) ou resumo de negócio.

4. **Painel de Métricas e KPIs Globais:**
   - **191 novidades** catalogadas no repositório, **82 em GA (Produção)**, **58 lançamentos de modelos de IA** e **13 edições semanais** publicadas.

---

## 🚀 Como Executar e Visualizar Localmente

### 1. Visualização em Markdown
Você pode visualizar diretamente os arquivos `.md` na sua IDE (como Antigravity, VS Code, Cursor) usando a pré-visualização integrada de Markdown:
- Atalho padrão: `Ctrl + Shift + V` ou `Ctrl + K V`

### 2. Abertura Direta no Navegador
Você pode abrir o arquivo `wiki_preview.html` diretamente no seu navegador padrão:

```bash
xdg-open "/home/ricdealm/Novidades AI/wiki_preview.html"
# ou diretamente via Google Chrome:
google-chrome "/home/ricdealm/Novidades AI/wiki_preview.html"
```

Ou cole a URL direta no navegador:
```
file:///home/ricdealm/Novidades%20AI/wiki_preview.html
```

### 3. Servidor Local HTTP em Python (Recomendado)
Para servir a aplicação e navegar como em uma intranet corporativa:

```bash
cd "/home/ricdealm/Novidades AI"
python3 -m http.server 8080
```

Em seguida, acesse no navegador: [http://localhost:8080/wiki_preview.html](http://localhost:8080/wiki_preview.html)

---

## 🔄 Histórico de Atualizações

- **09/11/2026 (Edição 09/11/2026 - 19 novos lançamentos):**
  - Adição do arquivo `novidades_google_ai_09-11-2026.md` com 19 novidades:
    - **Modelos de IA:** Gemini Omni 1.2 Flash em GA (`gemini-omni-1.2-flash`), Interactions API com decodificação estendida (Long Decodes de até 1.048.576 tokens) para Gemini 4 Argon (GA) e Tool Retrieval (EAP), AlphaGenome (`alphagenome-004`) com streaming unificado gRPC/HTTP/2 (GA) e implantação de modelos ajustados Gemini 3.x em endpoints globais via `models:copy` (GA);
    - **Infraestrutura e Plataforma de Agentes:** Interface dedicada do Memory Bank no Console Google Cloud, Throughput Provisionado para modelos com ajuste fino supervisionado (GA), CodeMender v0.18.0 com limites de segurança em sessões `cm verify` e benchmark aberto Physical-Engineering's Last Exam (PLE) em parceria com a Mercor;
    - **Dados, Inteligência Documental e Análise Agêntica:** Funções SQL nativas `AI.PARSE_DOCUMENT` e `AI.CHUNK_DOCUMENT` no BigQuery (GA), agregação semântica em escala com `AI.AGG` no BigQuery, previsões zero-shot no Pandas com o acessador `.bigquery` do BigFrames e avanços no Agentic Data Cloud (System of Action com Spanner, AlloyDB e BigQuery);
    - **Conectores e Integrações (Gemini Enterprise App):** Conector de armazenamento de dados Adobe (Public Preview) e Conector Federado para Salesforce CRM em GA;
    - **Gestão de IA, FinOps e Governança:** Controle de disponibilidade de modelos por política organizacional de localização de recursos (`Resource Location Policies`), créditos pré-pagos para assinaturas Pay-as-you-go e excedentes (GA), comutação de equipes no app móvel, atualização do modelo de geração de vídeo para Gemini Omni 1.2 Flash (GA) e cronograma de transição das licenças integradas do Gemini Code Assist (vigência até 31/03/2027).
- **02/11/2026 (Edição 02/11/2026 - 13 novos lançamentos):**
  - Adição do arquivo `novidades_google_ai_02-11-2026.md` com 13 novidades:
    - **Modelos de IA:** Gemini 4 Carbon (Frontier Model para cibersegurança e raciocínio de longo alcance, 1º lugar no Artificial Analysis Intelligence Index v5.0), Gemini Robotics ER 2 (Preview), xAI Grok 4.7 (GA) e Gemini 3.8 Flash TTS / Flash-Lite TTS (GA);
    - **Infraestrutura e Plataforma de Agentes:** Antigravity Plugin Marketplace (`plugin.json`) e ferramenta de Computer Use em GA com governança Human-in-the-Loop (`configurableComputerUseToolSafetyPolicies`);
    - **Segurança e Governança:** Ambient Quality Agent (AQuA) para observabilidade contínua e diagnóstico de causa-raiz de agentes em produção;
    - **Gemini Enterprise App, Conectores e FinOps:** Gemini Notebook Enterprise Visual Refresh (GA), parceria estratégica ServiceNow Action Fabric e Google Cloud, Workspace Connectors v2 baseados em rMCP (ações no Docs, Sheets e Slides), conectividade VPC e egress com IP estático para servidores MCP customizados (GA), recursos de FinOps e previsão orçamentária no painel administrativo e confirmação da descontinuação do Gemini 3.6 Flash em 19/11/2026.
- **26/10/2026 (Edição 26/10/2026 - 12 novos lançamentos):**
  - Adição do arquivo `novidades_google_ai_26-10-2026.md` com 12 novidades:
    - **Modelos de IA:** Modelos OpenAI nativos no Google Cloud (`GPT-6 Astra`, `GPT-6.1 Sol` e `GPT-6 Luna` em Private Preview), Claude Models no Google Cloud gerenciados pela Anthropic (`claude.googleapis.com` em GA), Gemini 3.5 Transcribe ASR em tempo real e lote (GA) e Gemini 4 Argon em regiões com Data Residency Zero (DRZ);
    - **Infraestrutura e Plataforma de Agentes:** Virtualização aninhada (`/dev/kvm`) no GKE Autopilot e Custom Compute Classes (GA) e CodeMender v0.16.0 com varredura profunda padrão (`cm find --deep`) e diagnóstico de saúde (`cm health`) em GA;
    - **Gemini Enterprise App, Conectores, Gestão e CX:** Data Cloud Connectors 1P via MCP para BigQuery, Spanner, Cloud SQL e AlloyDB (Preview), BigQuery Conversational Analytics (GA), limites de cota por usuário único (GA), suporte ao Antigravity Enterprise Gateway (GA), Gemini 4 Argon como modelo padrão no AlphaEvolve e evolução do Gemini for Customer Experience (CX Agent Studio).
- **19/10/2026 (Edição 19/10/2026 e Consolidação de 10 Semanas):**
  - Adição do arquivo `novidades_google_ai_19-10-2026.md` com 11 novos lançamentos:
    - Gemini 4 Argon (GA) e Gemini 4 Argon Cyber Permissive (GA);
    - Priority PayGo para Gemini Nano Banana 2.1 (GA);
    - DeepSeek-V4.1-Flash gerenciado no Model Garden (Public Preview);
    - TimesFM 3.0 para previsão multivariada no BigQuery via `AI.FORECAST`;
    - K8s Bridge open source para GKE (integração Slurm Operator + Kueue);
    - Gemini 4 Argon no AlphaEvolve e CodeMender 0.14/0.15 com SARIF 2.1.0;
    - Claude Opus 5.5 e Claude Sonnet 5.5 no seletor web do Gemini Enterprise (GA);
    - Gemini 4 Argon no Web App, Mobile e ferramentas corporativas;
    - Chips de citação para fontes MCP customizadas via REST API;
    - Novos conectores para Confluence/Jira Data Center, Salesforce, MS Teams e Notion;
    - Google Flow for Enterprise no Private Preview.
  - Atualização do visualizador `wiki_preview.html` abrangendo as **10 edições semanais** e **147 novidades catalogadas**.
  - Recálculo dos KPIs: 61 itens em GA, 46 modelos e 10 semanas.
- **12/10/2026 (Consolidação Multi-Edições - 136 Itens):**
  - Incorporação dos arquivos semanais de julho a outubro de 2026.
  - Implementação dos filtros combinados por semana e categorias técnicas.
- **04/10/2026 (Lançamento Inicial):**
  - Criação da interface interativa da Wiki (`wiki_preview.html`).
