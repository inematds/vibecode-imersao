# PLANO: Imersao Vibe Coding - Do Zero ao SaaS com IA

**Formato:** Imersao 3 dias / 6 turnos / 6 trilhas
**Objetivo:** Construir um SaaS de assistentes com IA usando Vibe Coding
**Entrega final:** SaaS funcional com agentes, deploy e monetizacao
**URL:** https://inematds.github.io/vb-imersao/

---

## ESTRUTURA: 6 TRILHAS (1 por turno)

### Trilha 1 - Mentalidade e Metodo de Vibe Coding (Emerald)
*Dia 1 / Turno 1 - Como pensar e estruturar projetos com IA*

6 topicos:
1. O que e Vibe Coding em 2026 - Karpathy, evolucao para Agentic Engineering, Vibe Shipping
2. Da Ideia ao Software - Problema > Usuario > Solucao > MVP
3. Escopo e Definicao de Produto - MVP, fluxos, telas, limites
4. Prompts Estruturados para Construcao - [Contexto+Instrucao+Restricao+Formato]
5. Erros Comuns em Projetos com IA - 45% vulnerabilidades, 5 erros fatais
6. Exercicio: Definir seu SaaS - Frase do produto, fluxo, telas, limites

Dados pesquisa: 92% devs US usam IA, 41% codigo global gerado por IA, de vibe coding pra vibe shipping

---

### Trilha 2 - Arquitetura da Plataforma de Agentes (Blue)
*Dia 1 / Turno 2 - Estrutura base do projeto*

6 topicos:
1. Arquitetura de Plataformas de Agentes - app, agents, prompts, skills, tools, memory
2. Estrutura de Pastas Profissional - Separacao de concerns que escala
3. Configuracao de APIs e Variaveis - .env, secrets, multiplos providers
4. Contexto Global vs por Agente - Quando compartilhar vs isolar
5. Fluxo Padrao de Execucao - Entrada > Decisao > Execucao > Saida
6. Exercicio: Criar Estrutura Base - Repo, pastas, .env, primeiro agente

Dados pesquisa: A-tier architecture (Akka), evento-driven, 10M TPS, multi-tenant isolation

---

### Trilha 3 - Construcao do SaaS (Purple)
*Dia 2 / Turno 3 - Produto funcional*

6 topicos:
1. Autenticacao e Onboarding - Login, registro, primeiro acesso, Supabase Auth
2. Dashboard e Interface Principal - Layout, navegacao, UX para apps com IA
3. System Prompts e Fluxo da Aplicacao - Entrada > Processamento > Saida
4. Upload Multimodal - PDF, imagem, video, processamento de arquivos
5. Estados do Sistema e Historico - Carregando, processando, erro, concluido
6. Exercicio: SaaS Funcional - Interface completa com auth, dashboard, fluxo

Dados pesquisa: Conversation-centered vs transaction-centered, outcome-based pricing (Gartner 2030)

---

### Trilha 4 - Agentes, MCP e Skills (Amber)
*Dia 2 / Turno 4 - Inteligencia no sistema*

6 topicos:
1. O que sao Agentes de IA - Automacao vs agentes inteligentes, loops de decisao
2. Multiagentes e Orquestracao - Executor, Analista, Revisor, pods especializados
3. Skills e Tools - Capacidades especializadas, schemas, registro
4. MCP (Model Context Protocol) - Anthropic, Host/Client/Server, conectores
5. Memoria e Handoff entre Agentes - Curta vs longa, passagem de contexto, tenant isolation
6. Exercicio: Integrar Agentes - Criar 2+ agentes com skill + MCP

Dados pesquisa: MCP open standard Anthropic, milhares de conectores, SDKs Python/TS/Java, 42% empresas com agentic em producao

---

### Trilha 5 - Assistentes e Multibots (Teal)
*Dia 3 / Turno 5 - Plataforma de assistentes*

6 topicos:
1. Assistente Unico vs Multiplos - Quando usar cada arquitetura
2. Arquitetura Multibot - Orquestracao de bots especialistas, router
3. Bots Especialistas - Marketing, vendas, atendimento, conteudo, operacao
4. OpenClaw e ClaudeClaw - Frameworks de referencia para bots pessoais
5. Integracao com Canais - Web, Telegram, WhatsApp, multichannel
6. Exercicio: Implementar Multibot - Sistema multibot funcional

Dados pesquisa: LangBot (10+ platforms), Botpress (10 canais), Manus AI no Telegram, OpenClaw open-source

---

### Trilha 6 - Seguranca, Billing e Operacao (Rose)
*Dia 3 / Turno 6 - Producao e monetizacao*

6 topicos:
1. Seguranca de Prompts e API Keys - Injection, vazamento, protecao
2. Autenticacao e Autorizacao - RBAC, JWT, rotas protegidas
3. Logs, Observabilidade e Monitoramento - O que logar, debugar, alertas
4. Pagamentos e Planos SaaS - Stripe, planos, trial, usage-based
5. Landing Page e Analytics - Conversao, metricas, tracking
6. Exercicio: Deploy Final - App publicada com landing, billing, logs

Dados pesquisa: Governance-as-Code, Digital DNA, usage/outcome-based pricing, Zero-Copy Architecture

---

## RESUMO

| Trilha | Cor | Turno | Topicos | Entrega |
|--------|-----|-------|---------|---------|
| T1 Mentalidade | Emerald | Dia 1 T1 | 6 | Definicao do SaaS |
| T2 Arquitetura | Blue | Dia 1 T2 | 6 | Estrutura base |
| T3 Construcao | Purple | Dia 2 T3 | 6 | SaaS funcional |
| T4 Agentes | Amber | Dia 2 T4 | 6 | Agentes integrados |
| T5 Multibots | Teal | Dia 3 T5 | 6 | Sistema multibot |
| T6 Operacao | Rose | Dia 3 T6 | 6 | Deploy final |
| **TOTAL** | | **6** | **36** | **6** |
