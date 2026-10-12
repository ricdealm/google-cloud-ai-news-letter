# Google Cloud AI Newsletter & Base de Conhecimento

Repositório central de documentação técnica e boletins informativos periódicos sobre as atualizações, lançamentos e anúncios da stack de inteligência artificial do Google (Gemini Enterprise Agent Platform, Model Garden, Agent Development Kit - ADK, Gemini Enterprise App e FinOps).

🔗 **Repositório Remoto no GitHub:** [https://github.com/ricdealm/google-cloud-ai-news-letter.git](https://github.com/ricdealm/google-cloud-ai-news-letter.git)

---

## 🏛️ Estrutura e Arquitetura do Repositório

O projeto foi estruturado para suportar publicação contínua em formato Markdown (pronto para exportação para Confluence, GitHub Wiki, Notion ou e-mails corporativos) aliado a um visualizador interativo em HTML/Tailwind com suporte a filtros dinâmicos:

```
Novidades AI/
├── novidades_google_ai_12-10-2026.md  # Boletim técnico da semana de 12/10/2026 (05 a 12/out/2026)
├── novidades_google_ai_04_10_2026.md  # Boletim técnico da semana de 04/10/2026 (22/set a 03/out/2026)
├── wiki_preview.html                  # Visualizador interativo em layout Wiki com filtros por semana e categoria
└── Readme.md                          # Este documento (arquitetura, funcionalidades e execução)
```

### 📦 Funcionalidades da Aplicação (`wiki_preview.html`)
1. **Filtro Temporal por Semana (Edição):**
   - **Todas as Semanas:** Visão unificada com 24 lançamentos.
   - **Semana 12/10/2026:** Foco nos 9 novos lançamentos mais recentes.
   - **Semana 04/10/2026:** Histórico consolidado com os 15 lançamentos anteriores.
2. **Filtro por Categorias Técnicas:**
   - 🧠 **Modelos de IA:** Anúncios da família Gemini, Anthropic Claude no Model Garden/Antigravity, parceiros (xAI Grok, Meta Muse).
   - 🛠️ **Plataforma de Agentes & Infra:** ADK (Model Consult, Deferred Scheduling), AlloyDB AI (BM25 + vetores), BigQuery / Spanner Iceberg, Interactions API.
   - 📱 **Gemini Enterprise App:** O novo agente corporativo do Gemini (Gemini at Work), autorouting para Flash 3.8, Grounding com Exa.
   - ⚙️ **FinOps & Gestão:** Expansão PAYG para Frontline/EDU, novos tiers sem ramp limits, reestruturação self-service de Provisioned Throughput e painel de custos no Studio.
3. **Busca Rápida em Tempo Real:** Pesquisa instantânea por nome de modelo, SKU, tecnologia, tag ou impacto de negócio.
4. **Painel Executivo e Métricas (KPIs):** Total cadastrado, itens em GA (Produção), modelos Frontier e soluções de governança.

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
- **12/10/2026:** 
  - Adição do boletim técnico `novidades_google_ai_12-10-2026.md` com 9 novas atualizações (Gemini Nano Banana 2.1 GA, Claude Haiku 5.5 GA, Claude Opus/Sonnet no Antigravity, ADK Model Consult e Deferred Scheduling, AlloyDB BM25, Spanner Iceberg Runtime Catalog, Gemini at Work e expansão de PAYG).
  - Atualização do visualizador `wiki_preview.html` com suporte a filtros combinados por **Semana** e **Categoria**, busca textual dinâmica, atualização dos KPIs e estado vazio personalizado.
  - Configuração do repositório Git e envio para o GitHub (`https://github.com/ricdealm/google-cloud-ai-news-letter.git`).
- **04/10/2026:**
  - Sincronização do HTML (`wiki_preview.html`) com o boletim `novidades_google_ai_04_10_2026.md`.
  - Implementação da interface interativa inicial da Wiki com filtros e métricas.
