# Visual Studio — Assistente de IA Pessoal

<p align="center">
  <svg width="120" height="120" viewBox="0 0 120 120" fill="none" xmlns="http://www.w3.org/2000/svg">
    <rect width="120" height="120" rx="24" fill="url(#vs-g)"/>
    <defs>
      <linearGradient id="vs-g" x1="0%" y1="0%" x2="100%" y2="100%">
        <stop offset="0%" stop-color="#3b82f6"/>
        <stop offset="100%" stop-color="#1d4ed8"/>
      </linearGradient>
    </defs>
    <text x="60" y="82" font-family="system-ui,-apple-system,sans-serif" font-size="56" font-weight="700" fill="#ffffff" text-anchor="middle" letter-spacing="-2">VS</text>
  </svg>
</p>

<p align="center">
  <strong>Seu assistente de IA rodando no seu próprio servidor</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Node.js-22%2B-green?style=for-the-badge&logo=node.js" alt="Node.js 22+">
  <img src="https://img.shields.io/badge/Interface-PT--BR-009c3b?style=for-the-badge" alt="PT-BR">
  <a href="https://www.visualstudio.com.br"><img src="https://img.shields.io/badge/Site-visualstudio.com.br-3b82f6?style=for-the-badge" alt="Site"></a>
</p>

---

**Visual Studio** é um gateway de IA pessoal que você instala nos seus próprios servidores. Ele conecta assistentes de inteligência artificial aos canais de mensagem que você já usa, com interface web completa em português brasileiro.

## ✨ Funcionalidades

- **Multi-canal** — WhatsApp, Telegram, Slack, Discord, Signal, iMessage, Microsoft Teams, Matrix e muito mais
- **Modelos locais** — suporte nativo a Ollama, LM Studio e outros provedores locais
- **Interface em PT-BR** — painel web completo em português com tema azul
- **Auto-hospedado** — seus dados ficam no seu servidor, não em nuvens de terceiros
- **Extensível** — mais de 140 extensões/plugins disponíveis
- **Voz** — fala e escuta no macOS, iOS e Android
- **Canvas** — renderização de conteúdo interativo em tempo real

## 🚀 Instalação rápida

### Pré-requisitos

- Node.js 22.19+ (recomendado: Node 24)
- pnpm

### Via npm

```bash
npm install -g visual-studio
visual-studio onboard
```

### Via Docker

```bash
docker compose up -d
```

O gateway sobe na porta `18789` por padrão. Acesse a interface web em `http://localhost:18789`.

### Desenvolvimento local

```bash
pnpm install
pnpm dev
```

## 📁 Estrutura do projeto

```
visual-studio/
├── src/              # Backend principal (TypeScript/Node.js)
│   ├── agents/       # Motor de agentes de IA
│   ├── cli/          # Interface de linha de comando
│   ├── daemon/       # Gerenciamento de serviços
│   └── gateway/      # Servidor HTTP/WebSocket
├── ui/               # Interface web (Lit + Vite)
│   └── src/
│       ├── i18n/     # Internacionalização (PT-BR padrão)
│       └── ui/       # Componentes da interface
├── extensions/       # Plugins de canais e provedores
└── packages/         # Pacotes internos compartilhados
```

## 🔧 Configuração

Execute o assistente de configuração para criar sua configuração inicial:

```bash
visual-studio onboard
```

O assistente vai guiá-lo passo a passo pela configuração do gateway, canais e modelos de IA.

## 🐳 Deploy com Docker

```bash
# Suba o container
docker compose up -d
```

Configure as variáveis de ambiente no arquivo `.env` antes de subir. O arquivo `docker-compose.yml` documenta todas as opções disponíveis.

## 🤖 Provedores de IA suportados

- **Nuvem**: OpenAI, Anthropic Claude, Google Gemini, AWS Bedrock, Azure OpenAI
- **Local**: Ollama, LM Studio, llama.cpp
- **Outros**: Groq, DeepSeek, Mistral, Qwen, e mais

## 📱 Canais de mensagem

WhatsApp · Telegram · Slack · Discord · Signal · iMessage · Microsoft Teams · Google Chat · Matrix · Feishu · LINE · Mattermost · Nextcloud Talk · Synology Chat · IRC · Twitch · e mais

---

<p align="center">
  <a href="https://www.visualstudio.com.br">www.visualstudio.com.br</a>
</p>
