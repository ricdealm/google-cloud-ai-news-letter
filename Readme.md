# Google Cloud AI Newsletter & Base de Conhecimento

Repositório central de documentação técnica e boletins informativos periódicos sobre as atualizações, lançamentos e anúncios da stack de inteligência artificial do Google (Gemini Enterprise Agent Platform, Model Garden, Agent Development Kit - ADK, Gemini Enterprise App, Segurança & Governança e FinOps).

🔗 **Repositório Remoto no GitHub:** [https://github.com/ricdealm/google-cloud-ai-news-letter.git](https://github.com/ricdealm/google-cloud-ai-news-letter.git)

---

## 🏛️ Estrutura e Arquitetura do Repositório

O projeto foi estruturado para suportar publicação contínua em formato Markdown (pronto para exportação para Confluence, GitHub Wiki, Notion ou e-mails corporativos) aliado a um visualizador interativo em HTML/Tailwind com suporte a filtros dinâmicos e busca instantânea:

```
Novidades AI/
├── novidades_google_ai_19-10-2026.md  # Edição de 19/10/2026 (13 a 19/out/2026) - 11 itens (Mais recente)
├── novidades_google_ai_12-10-2026.md  # Edição de 12/10/2026 (05 a 12/out/2026) - 9 itens
├── novidades_google_ai_04_10_2026.md  # Edição de 04/10/2026 (22/set a 03/out/2026) - 15 itens
├── novidades_google_ai_22-09-2026.md  # Edição de 22/09/2026 (14 a 21/set/2026) - 14 itens
├── novidades_google_ai_13-09-2026.md  # Edição de 13/09/2026 (19/ago a 12/set/2026) - 21 itens
├── novidades_google_ai_18-08-2026.md  # Edição de 18/08/2026 (09 a 17/ago/2026) - 13 itens
├── novidades_google_ai_08-08-2026.md  # Edição de 08/08/2026 (02 a 08/ago/2026) - 15 itens
├── novidades_google_ai_01-08-2026.md  # Edição de 01/08/2026 (21 a 31/jul/2026) - 16 itens
├── novidades_google_ai_20-07-2026.md  # Edição de 20/07/2026 (02 a 20/jul/2026) - 11 itens
├── novidades_google_ai_01-07-2026.md  # Edição de 01/07/2026 (16 a 30/jun/2026) - 22 itens
├── wiki_preview.html                  # Visualizador interativo em layout Wiki com filtros por semana e categoria (147 novidades)
└── Readme.md                          # Este documento (arquitetura, funcionalidades e execução)
```

---

## 📦 Funcionalidades da Aplicação (`wiki_preview.html`)

1. **Filtro Temporal por Semana (10 Edições Catalogadas):**
   - **Todas as Semanas:** Visão unificada com o acervo completo de **147 lançamentos**.
   - **Filtro Rápido no Topo e Dropdown:** Seleção direta entre qualquer uma das 10 semanas (01/07/2026 até 19/10/2026).
   - **Sidebar com Navegação e Contadores:** Menu lateral esquerdo com links âncora e contagem individual de novidades por edição.

2. **Filtro por Categorias Técnicas:**
   - 🧠 **Modelos de IA (46 lançamentos):** Gemini 4 Argon (GA) e Cyber Permissive, Gemini Nano Banana 2.1, DeepSeek-V4.1-Flash no Model Garden, Claude Opus/Sonnet 5.5, Llama e parceiros.
   - 🛠️ **Plataforma de Agentes & Infra (43 lançamentos):** TimesFM 3.0 no BigQuery (`AI.FORECAST`), K8s Bridge open source para GKE (Slurm Operator + Kueue), Gemini 4 Argon no AlphaEvolve e CodeMender, Agent Development Kit (ADK), AlloyDB AI e Spanner Iceberg Catalog.
   - 🛡️ **Segurança & Governança (14 lançamentos):** Model Armor, Content Safety Guardrails, VPC Service Controls, Data Residency e Criptografia CMEK.
   - 📱 **Gemini Enterprise App & Conectores (36 lançamentos):** Gemini 4 Argon no Web/Mobile App, Claude Opus/Sonnet 5.5 no seletor do app, citações customizadas via MCP (`citation_mappings`), conectores Jira/Confluence/Salesforce/Teams/Notion no Workflow Builder e Google Flow for Enterprise.
   - ⚙️ **FinOps & Gestão de Modelos (8 lançamentos):** Priority PayGo para Nano Banana 2.1, expansão PAYG para Frontline/EDU, Provisioned Throughput sem ramp limits, painéis de auditoria de custo e quota dinâmicos.

3. **Busca Textual em Tempo Real:**
   - Pesquisa instantânea inteligente por nome de modelo, tecnologia, autoroute, tag de estágio (GA, Preview, Open Source) ou resumo de negócio.

4. **Painel de Métricas e KPIs Dinâmicos:**
   - Contador de novidades visíveis filtradas em tempo real.
   - Métricas globais: 147 novidades, 61 em GA (Produção), 46 modelos de IA e 10 edições semanais publicadas.

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
