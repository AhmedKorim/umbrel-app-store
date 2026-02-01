# Korrim Umbrel App Store

A custom app store for Umbrel OS with curated applications for self-hosted infrastructure.

## Apps

### OpenClaw - Personal AI Assistant

OpenClaw is a personal AI assistant you run on your own devices. It integrates with multiple communication channels and supports various AI models.

**Features:**
- Multi-channel support (WhatsApp, Telegram, Slack, Discord, Signal, iMessage, Teams, and more)
- Voice and canvas interaction
- WebSocket-based gateway control plane
- Multi-agent routing with isolated workspaces
- Compatible with Anthropic Claude, OpenAI, and other AI models
- Self-hosted and privacy-focused

**Installation:**
1. Add this app store to your Umbrel OS
2. Install OpenClaw from the store
3. Configure your AI provider credentials (optional but recommended)
4. Access the web UI at port 18789

**Configuration:**
OpenClaw supports several optional environment variables for AI authentication:

- `OPENCLAW_GATEWAY_TOKEN`: Gateway authentication token (auto-generated if not provided)
- `CLAUDE_AI_SESSION_KEY`: Anthropic Claude AI session key for OAuth authentication
- `CLAUDE_WEB_SESSION_KEY`: Anthropic Claude web session key
- `CLAUDE_WEB_COOKIE`: Anthropic Claude web cookie
- `TWILIO_ACCOUNT_SID`: Twilio account SID for WhatsApp integration
- `TWILIO_AUTH_TOKEN`: Twilio auth token for WhatsApp integration
- `TWILIO_WHATSAPP_FROM`: Twilio WhatsApp number (format: whatsapp:+1234567890)

**Getting Started:**
After installation, you can:
1. Use the web Control UI at `http://your-umbrel-ip:18789`
2. Run the onboarding wizard to configure channels and AI models
3. Connect your preferred communication channels
4. Start interacting with your AI assistant

**Documentation:**
- Official Docs: https://docs.openclaw.ai
- GitHub: https://github.com/openclaw/openclaw
- Support: https://docs.openclaw.ai/start/faq

## Adding to Umbrel

To add this app store to your Umbrel OS:

1. Navigate to your Umbrel dashboard
2. Go to App Store settings
3. Add custom app store: `https://github.com/korrim/umbrel-app-store`

## Contributing

This is a personal app store for custom applications. Feel free to fork and create your own.

## License

This app store configuration follows the same license as the original template.
