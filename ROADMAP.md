# Morning Brief - Roadmap

Motor: **OpenClaw** (agentes Voyager + Mercury)
RVM Project ID: **17**

---

## Fase 1 - Fundacao & Infra
- [x] Setup Node.js + ESM + dotenv
- [ ] Conectar ao Convex (OpenClaw shared)
- [ ] Criar soul do agente briefing no OpenClaw
- [ ] Configurar variaveis de ambiente (.env)

## Fase 2 - Fontes de Dados
- [ ] Integrar Google Calendar API (OAuth2 / service account)
- [ ] Integrar OpenWeather API (cidade configuravel)
- [ ] Integrar NewsAPI ou RSS feeds de IA (TheVerge, ArsTechnica, TechCrunch, HF blog)
- [ ] Conectar ao RVM API para tarefas pendentes
- [ ] Criar modulo de coleta unificado (paralelo)

## Fase 3 - Motor de Briefing
- [ ] Criar prompt template (Agenda, Tarefas, Clima, Noticias AI, Frase motivacional)
- [ ] Integrar com OpenClaw Voyager para pesquisa
- [ ] Usar Mercury para redacao do briefing
- [ ] Enviar briefing via Telegram Bot (MarkdownV2)

## Fase 4 - Automacao & Deploy
- [ ] Configurar node-cron para 7h BRT (`0 7 * * *`)
- [ ] Deploy no Hetzner via pm2
- [ ] Heartbeat no RVM
- [ ] Fallback graceful se API falhar

## Fase 5 - Polish & Extras
- [ ] Comando `/brief` no Telegram (sob demanda)
- [ ] Historico de briefings no Convex
- [ ] Metricas de uso no RVM dashboard
- [ ] Personalizacao por usuario (fontes, cidade, horario)

---

**Total: 21 tasks | 5 fases**
