# Korrim Umbrel App Store

A custom app store for Umbrel OS with curated applications for self-hosted infrastructure.

## Apps

### OpenClaw - Personal AI Assistant (Telegram Optimized)

OpenClaw is a personal AI assistant you run on your own devices. This installation is optimized for Telegram integration.

**Features:**
- Telegram integration (primary channel) - chat with your AI assistant directly in Telegram
- Multi-channel support (Slack, Discord, Signal, iMessage, Teams, and more)
- Voice and canvas interaction
- WebSocket-based gateway control plane
- Multi-agent routing with isolated workspaces
- Compatible with Anthropic Claude, OpenAI, and other AI models
- Self-hosted and privacy-focused

**Installation:**
1. Add this app store to your Umbrel OS
2. Install OpenClaw from the store
3. Configure your AI provider credentials (optional but recommended)
4. Set up Telegram bot (see below)
5. Access the web UI at port 18789

**Telegram Setup:**
1. Open Telegram and search for @BotFather
2. Send `/newbot` and follow the instructions to create your bot
3. Copy the bot token provided by BotFather
4. Access the OpenClaw web UI at `http://your-umbrel-ip:18789`
5. Navigate to channel settings and add your Telegram bot token
6. Start a conversation with your bot in Telegram

**Configuration:**
OpenClaw supports several optional environment variables for AI authentication:

- `OPENCLAW_GATEWAY_TOKEN`: Gateway authentication token (auto-generated if not provided)
- `CLAUDE_AI_SESSION_KEY`: Anthropic Claude AI session key for OAuth authentication (recommended)
- `CLAUDE_WEB_SESSION_KEY`: Anthropic Claude web session key
- `CLAUDE_WEB_COOKIE`: Anthropic Claude web cookie

**Getting Started:**
After installation, you can:
1. Use the web Control UI at `http://your-umbrel-ip:18789`
2. Run the onboarding wizard to configure Telegram and AI models
3. Start chatting with your AI assistant in Telegram
4. Use voice messages and other interactive features

**Documentation:**
- Official Docs: https://docs.openclaw.ai
- GitHub: https://github.com/openclaw/openclaw
- Support: https://docs.openclaw.ai/start/faq

## Adding to Umbrel

To add this app store to your Umbrel OS:

1. Navigate to your Umbrel dashboard
2. Go to App Store settings
3. Add custom app store: `https://github.com/AhmedKorim/umbrel-app-store`

## Contributing

This is a personal app store for custom applications. Feel free to fork and create your own.

## License

This app store configuration follows the same license as the original template.
