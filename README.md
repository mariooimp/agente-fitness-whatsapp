# Agente Fitness para WhatsApp

Agente de IA especializado em fitness integrado ao WhatsApp,
com memória de conversação persistente.

## Problema que resolve
Personal trainers e academias recebem diariamente dezenas
de perguntas repetitivas no WhatsApp — treinos, dietas,
exercícios, suplementação. Esse agente automatiza esse
atendimento de forma inteligente, mantendo contexto da
conversa com cada usuário.

## Arquitetura
Webhook → Dados → Switch → AI Agent → Send Seen → Send Text
                               ↓
                   Google Gemini + Redis Memory

## Tecnologias
- N8N — orquestração do fluxo de automação
- Google Gemini API — modelo de linguagem
- Redis — memória persistente de conversação
- WAHA — integração com WhatsApp
- Docker — containerização do ambiente

## Funcionalidades
- Responde dúvidas sobre treinos e exercícios
- Orienta sobre alimentação e dieta
- Tira dúvidas sobre suplementação
- Mantém contexto da conversa com cada usuário
- Respostas objetivas e especializadas em fitness

## Como executar
1. Clone o repositório
2. Configure as variáveis de ambiente com suas chaves de API
3. Importe o arquivo `flow.json` no N8N
4. Suba o ambiente com Docker
