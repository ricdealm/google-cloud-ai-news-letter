## 🚀 Gemini Enterprise Agent Platform

### 🧠 Modelos de IA

| Funcionalidade / Atualização | Detalhes | Link de Documentação Pública |
| :--- | :--- | :--- |
| **Otimização do Qwen 3.5 MoE em TPUs Ironwood v7x (Informativo)** | Playbook técnico focado na otimização de execução do modelo de mistura de especialistas (**Mixture-of-Experts - MoE**) **Qwen 3.5-397B** em aceleradores de hardware Ironwood (TPU v7x) utilizando kernels Pallas/JAX.<br><br>**Por que isso importa:** Supera os desafios físicos de largura de banda de memória usando sharding híbrido (DP=8 + EP=8), alcançando desempenho **3.1x superior em geração (Decode)** e **4.7x em processamento de entrada (Prefill)**.<br><br>**Adoção Prática:** Integrações portadas nativamente para os frameworks de código aberto **vLLM** e **SGLang**, facilitando caminhos de produção corporativos em larga escala. | [Systems Engineering Playbook](https://developers.googleblog.com/systems-engineering-playbook-optimizing-qwen-35-397b-moe-on-ironwood-tpu7x/) |

---

### 🛠️ Infraestrutura e Plataforma de Agentes (Agent Platform)

| Funcionalidade / Atualização | Detalhes | Link de Documentação Pública |
| :--- | :--- | :--- |
| **Memory Profiles no Memory Bank (GA)** | Lançamento em **General Availability (GA)** dos perfis de memória. Permite a geração de perfis estruturados com esquemas estáticos populados e atualizados por LLMs.<br><br>**Por que isso importa:** Garante que os agentes tenham acesso imediato e de **baixa latência** a informações corporativas dinâmicas.<br><br>**Impacto:** Elimina a necessidade de operações de busca (search) caras e lentas durante as sessões de conversação. | [Memory profiles](https://docs.cloud.google.com/gemini-enterprise-agent-platform/scale/memory-bank/profiles) |
| **Arquitetura Prompts-as-Code (Informativo)** | Transição de prompts de sistema monolíticos para uma arquitetura modular de **Prompts-as-Code**.<br><br>**Por que isso importa:** À medida que agentes de IA avançam para produção, prompts monolíticos geram conflitos e falhas silenciosas de runtime.<br><br>**Solução:** Dividir prompts em arquivos de habilidades (*skills*) modulares usando um transpiler no build introduz resolução de dependências, validação estática e governança de **CI/CD** ao desenvolvimento de agentes. | [Building Scalable AI Agents](https://developers.googleblog.com/building-scalable-ai-agents-with-modular-prompt-transpilation/) |
| **Recap da Agent Factory: Engenharia 100X com Agentes de IA (Informativo)** | Insights sobre a transição massiva de IDEs tradicionais para **plataformas focadas primeiro em agentes** com o Google Antigravity 2.0.<br><br>**Por que isso importa:** Explora a nova realidade das revisões de código lideradas por IA e o uso de competências modulares (*skills*) para atingir produtividade de **100X** na engenharia. | [Agent Factory Recap](https://cloud.google.com/blog/topics/developers-practitioners/agent-factory-recap-100x-engineering-with-ai-agents-in-google-antigravity-20?e=48754805) |

---

### 🛡️ Segurança e Governança de IA

| Funcionalidade / Atualização | Detalhes | Link de Documentação Pública |
| :--- | :--- | :--- |
| **Uso Interno de IA na Segurança do Google Cloud (Informativo)** | Estudo de caso sobre como o time do Google Cloud Security utiliza agentes de IA especializados diretamente no **Ciclo de Vida de Desenvolvimento de Software (SDLC)**.<br><br>**Por que isso importa:** Demonstra a criação de guardrails autônomos e proativos que defendem aplicações em velocidade e escala inalcançáveis por revisões humanas. | [Google Cloud Security AI](https://cloud.google.com/blog/products/identity-security/cloud-ciso-perspectives-how-google-cloud-security-uses-ai-internally?e=48754805) |
| **4 Lições de Defesa Contra Ameaças de IA (Informativo)** | Artigo do CISO do Google Cloud, Chris Betz, abordando aprendizados práticos para usar a IA a favor dos defensores de segurança cibernética.<br><br>**Por que isso importa:** Orientações cruciais para desenhar defesas corporativas proativas usando **AI Threat Defense** contra ameaças de velocidade de máquina. | [4 Lessons of AI Threat Defense](https://cloud.google.com/blog/products/identity-security/cloud-ciso-perspectives-the-4-lessons-that-guided-ai-threat-defense?e=48754805) |

---

## 📱 Gemini Enterprise App – Julho de 2026

### 💬 Integrações e Acessibilidade

| Funcionalidade / Atualização | Detalhes | Link de Documentação Pública |
| :--- | :--- | :--- |
| **Bring Your Own Identity (BYOID) no Aplicativo Móvel (GA)** | O aplicativo móvel do Gemini Enterprise agora suporta oficialmente conexões com **provedores de identidade (IDPs) de terceiros** em General Availability (GA).<br><br>**Por que isso importa:** Permite que os usuários corporativos conectem o app móvel aos seus IDPs corporativos homologados sem precisar de inclusão em listas de permissões (allowlists), agilizando a governança e o acesso móvel seguro. | [Configure the mobile app](https://docs.cloud.google.com/gemini/enterprise/docs/configure-mobile-app) |

---

### 🗄️ Conectores de Dados (Data Stores) e Ações

| Funcionalidade / Atualização | Detalhes | Link de Documentação Pública |
| :--- | :--- | :--- |
| **Novos Data Stores e Suporte a Novas Ações (Preview)** | Lançamento em **Public Preview** de conectores adicionais de terceiros e ações de escrita nativas.<br><br>• **Novos Data Stores:** Aiwyn Tax, AllTrails, Autodesk Product Help, AWS Marketplace, Courtroom5, pg-aiguide, Taskrabbit, Twilio Docs, Viator e ZoomInfo.<br>• **Novas Ações Integradas:** Atualização de tickets no **Freshservice**, atualização de comentários de tickets no **Zoho Desk** e envio de feedbacks no **ZoomInfo**.<br><br>**Por que isso importa:** Permite realizar grounding rico e acionar automações diretamente sobre sistemas e repositórios de parceiros corporativos. | [Conectar Fonte de Terceiros](https://docs.cloud.google.com/gemini/enterprise/docs/connectors/connect-third-party-data-source)<br>[Autodesk Product Help](https://docs.cloud.google.com/gemini/enterprise/docs/connectors/autodesk-product-help)<br>[AWS Marketplace](https://docs.cloud.google.com/gemini/enterprise/docs/connectors/aws-marketplace)<br>[ZoomInfo](https://docs.cloud.google.com/gemini/enterprise/docs/connectors/zoominfo) |

---

### ⚙️ Gestão de IA e Modelos

| Funcionalidade / Atualização | Detalhes | Link de Documentação Pública |
| :--- | :--- | :--- |
| **Rebranding: NotebookLM Enterprise para Gemini Notebook Enterprise** | O produto NotebookLM Enterprise foi renomeado para **Gemini Notebook Enterprise**.<br><br>**Impacto técnico:** Nenhuma funcionalidade foi alterada e as APIs mantêm os mesmos endpoints herdados para evitar impactos de integração.<br><br>**Visualização:** O console de administração e o app web já refletem o novo nome, embora a página de faturamento e assinaturas ainda mostre temporariamente o termo legado. | [Create and manage notebooks (API)](https://docs.cloud.google.com/gemini/enterprise/notebooklm-enterprise/docs/api-notebooks) |
| **Google Nomeado Líder no IDC MarketScape 2026 (Informativo)** | Reconhecimento de destaque no relatório "IDC MarketScape: Worldwide Foundation Model Software 2026 Vendor Assessment" como um Líder do mercado global.<br><br>**Por que isso importa:** Valida a excelência comercial e a maturidade de engenharia da infraestrutura integrada do Google (conectando pesquisa do DeepMind com entrega estável). O relatório realça o valor da arquitetura unificada de agentes do **Gemini Enterprise** e a adaptabilidade da série **Gemini 3.5 (como o Gemini 3.5 Flash)** para lidar com fluxos agênticos complexos. | [Google Named a Leader in IDC MarketScape](https://cloud.google.com/blog/products/ai-machine-learning/google-named-a-leader-in-idc-marketscape?e=48754805) |
| **Pesquisa DORA: Medindo o ROI de IA no Desenvolvimento de Software (Informativo)** | Relatório focado em apresentar metodologias práticas para avaliar custos e retornos de negócios no uso de GenAI no desenvolvimento.<br><br>**Por que isso importa:** Ferramenta valiosa para apoiar decisores técnicos (CTOs, diretores) a alinhar investimentos de engenharia e mitigar atritos de adoção inicial. | [DORA: ROI of AI-assisted development](https://cloud.google.com/blog/products/ai-machine-learning/how-to-measure-the-business-value-of-generative-ai?e=48754805) |
