# Morning Brief

Assistente inteligente que gera um briefing personalizado todos os dias as 7h.

## O que faz

- Agenda do dia (Google Calendar)
- Tarefas pendentes (RVM + Todoist)
- Previsao do tempo (cidade configurada)
- Noticias de IA e tecnologia (curadoria automatica)
- Resumo executivo via Telegram

## Stack

- **Motor**: OpenClaw (agente Voyager para pesquisa, Mercury para redacao)
- **Runtime**: Node.js + cron job
- **Integracao**: Telegram Bot, Google Calendar API, OpenWeather API
- **Orquestracao**: Convex (shared com OpenClaw)
- **Deploy**: Hetzner VPS (pm2)

## Arquitetura

```
[Cron 7h] -> OpenClaw Gateway -> Voyager (pesquisa) -> Mercury (redacao)
                                      |
                                      v
                              [APIs externas]
                              - Google Calendar
                              - OpenWeather
                              - NewsAPI / RSS feeds IA
                              - RVM API (tarefas)
                                      |
                                      v
                              [Telegram] -> Red
```

## Status

Em desenvolvimento | Gerenciado pelo RVM Dashboard
