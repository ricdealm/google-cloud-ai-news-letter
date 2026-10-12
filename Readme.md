# Google Cloud AI Newsletter & Base de Conhecimento

Repositório central de documentação técnica e boletins informativos periódicos sobre as atualizações, lançamentos e anúncios da stack de inteligência artificial do Google (Gemini Enterprise Agent Platform, Model Garden, Agent Development Kit - ADK, Gemini Enterprise App, Segurança & Governança e FinOps).

🔗 **Repositório Remoto no GitHub:** [https://github.com/ricdealm/google-cloud-ai-news-letter.git](https://github.com/ricdealm/google-cloud-ai-news-letter.git)

---

## 🏛️ Estrutura e Arquitetura do Repositório

O projeto foi estruturado para suportar publicação contínua em formato Markdown (pronto para exportação para Confluence, GitHub Wiki, Notion ou e-mails corporativos) aliado a um visualizador interativo em HTML/Tailwind com suporte a filtros dinâmicos e busca instantânea:

```
Novidades AI/
├── novidades_google_ai_12-10-2026.md  # Edição de 12/10/2026 (05 a 12/out/2026) - 9 itens
├── novidades_google_ai_04_10_2026.md  # Edição de 04/10/2026 (22/set a 03/out/2026) - 15 itens
├── novidades_google_ai_22-09-2026.md  # Edição de 22/09/2026 (14 a 21/set/2026) - 14 itens
├── novidades_google_ai_13-09-2026.md  # Edição de 13/09/2026 (19/ago a 12/set/2026) - 21 itens
├── novidades_google_ai_18-08-2026.md  # Edição de 18/08/2026 (09 a 17/ago/2026) - 13 itens
├── novidades_google_ai_08-08-2026.md  # Edição de 08/08/2026 (02 a 08/ago/2026) - 15 itens
├── novidades_google_ai_01-08-2026.md  # Edição de 01/08/2026 (21 a 31/jul/2026) - 16 itens
├── novidades_google_ai_20-07-2026.md  # Edição de 20/07/2026 (02 a 20/jul/2026) - 11 itens
├── novidades_google_ai_01-07-2026.md  # Edição de 01/07/2026 (16 a 30/jun/2026) - 22 itens
├── wiki_preview.html                  # Visualizador interativo em layout Wiki com filtros por semana e categoria (136 novidades)
└── Readme.md                          # Este documento (arquitetura, funcionalidades e execução)
```

---

## 📦 Funcionalidades da Aplicação (`wiki_preview.html`)

1. **Filtro Temporal por Semana (9 Edições Catalogadas):**
   - **Todas as Semanas:** Visão unificada com o acervo completo de **136 lançamentos**.
   - **Filtro Rápido no Topo e Dropdown:** Seleção direta entre qualquer uma das 9 semanas (01/07/2026 até 12/10/2026).
   - **Sidebar com Navegação e Contadores:** Menu lateral esquerdo com links âncora e contagem individual de novidades por edição.

2. **Filtro por Categorias Técnicas:**
   - 🧠 **Modelos de IA (52 lançamentos):** Família Gemini (1.5 Flash/Pro, 2.0 Flash, Nano Banana), Claude 3.5 Sonnet / Haiku 5.5 / Opus no Antigravity e Model Garden, parceiros (xAI Grok, Meta Muse, Llama 3.1).
   - 🛠️ **Plataforma de Agentes & Infra (34 lançamentos):** Agent Development Kit (ADK), AlloyDB AI (BM25 + busca vetorial híbrida), BigQuery / Spanner Iceberg Runtime Catalog, Vertex AI Feature Store e RAG Engine.
   - 🛡️ **Segurança & Governança (14 lançamentos):** Model Armor, Content Safety Guardrails, VPC Service Controls para Vertex AI, Data Residency e Criptografia CMEK.
   - 📱 **Gemini Enterprise App & Conectores (30 lançamentos):** Gemini at Work, autoroute para Flash 3.8, conectores Grounding (Exa, Google Search, Google Workspace, Jira, ServiceNow, Salesforce).
   - ⚙️ **FinOps & Gestão de Modelos (6 lançamentos):** Expansão PAYG (Frontline/EDU), novos tiers de Provisioned Throughput sem ramp limits, painéis de auditoria de custo e quota dinâmicos no Studio.

3. **Busca Textual em Tempo Real:**
   - Pesquisa instantânea inteligente por nome de modelo, tecnologia, autoroute, tag de estágio (GA, Preview, Experimental) ou resumo de negócio.

4. **Painel de Métricas e KPIs Dinâmicos:**
   - Contador de novidades visíveis filtradas em tempo real.
   - Métricas globais de GA (Produção), Modelos Frontier e Soluções de Governança/Infra.

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

- **12/10/2026 (Consolidação Multi-Edições - 136 Itens):**
  - Incorporação de todos os 9 arquivos semanais cobrindo o período de julho a outubro de 2026 (`01/07`, `20/07`, `01/08`, `08/08`, `18/08`, `13/09`, `22/09`, `04/10` e `12/10`).
  - Totalização de **136 lançamentos e novidades técnicas** categorizadas e catalogadas.
  - Expansão do sistema de filtros no `wiki_preview.html`:
    - Dropdown seletor e botões rápidos para as 9 semanas.
    - Nova taxonomia de categorias incluindo **🛡️ Segurança & Governança**.
    - Navegação lateral (Sidebar) com links diretos para cada edição semanal e badge numérico de novidades.
  - Atualização dos KPIs do topo (Total de Itens, Produção GA, Modelos e Infra/Agentes).
- **12/10/2026 (Edição 12/10):**
  - Adição do boletim técnico `novidades_google_ai_12-10-2026.md` com 9 novas atualizações (Gemini Nano Banana 2.1 GA, Claude Haiku 5.5 GA, Claude Opus/Sonnet no Antigravity, ADK Model Consult e Deferred Scheduling, AlloyDB BM25, Spanner Iceberg Runtime Catalog, Gemini at Work e expansão de PAYG).
- **04/10/2026 (Lançamento Inicial):**
  - Criação da interface interativa da Wiki (`wiki_preview.html`) a partir de `novidades_google_ai_04_10_2026.md`.
  - Configuração do repositório Git e envio para o GitHub (`https://github.com/ricdealm/google-cloud-ai-news-letter.git`).
