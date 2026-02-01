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
3. Configure settings during installation (see below)
4. Access the web UI at port 18789

**Configuration (During Installation):**

When installing OpenClaw, you'll be prompted to configure:

1. **Claude AI Session Key** (Optional but recommended)
   - Your Anthropic Claude AI session key for OAuth authentication
   - Leave empty to configure later through the web UI
   - Recommended for best performance with Claude models

2. **Telegram Bot Token** (Required for Telegram integration)
   - Create a bot via @BotFather on Telegram
   - Send `/newbot` and follow the instructions
   - Copy the bot token (looks like `123456789:ABCdefGHI...`)
   - Paste it in the installation form
   - Leave empty to configure later through the web UI

3. **Gateway Token** (Optional)
   - Custom gateway authentication token
   - Leave empty to auto-generate a secure token

**Getting Started:**
After installation:
1. Find your Telegram bot and start a conversation
2. Access the web Control UI at `http://your-umbrel-ip:18789` for advanced configuration
3. Run the onboarding wizard to configure additional channels and AI models
4. Start chatting with your AI assistant in Telegram

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
