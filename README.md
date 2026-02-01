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
3. The app will automatically initialize with basic configuration
4. Access the web UI at port 18789 for further configuration

**Configuration (After Installation):**

After installing OpenClaw, you'll configure it through the web UI at `http://your-umbrel-ip:18789`:

1. **Telegram Setup:**
   - Open Telegram and search for @BotFather
   - Send `/newbot` and follow the instructions to create your bot
   - Copy the bot token (looks like `123456789:ABCdefGHI...`)
   - Access the OpenClaw web UI and add your Telegram bot token
   - Start a conversation with your bot in Telegram

2. **AI Provider Setup (Optional but recommended):**
   - Configure Anthropic Claude, OpenAI, or other AI providers
   - Use OAuth or API keys for authentication
   - Supports long-context models (200K+ tokens)

**Getting Started:**
After installation:
1. Set up SSH tunnel for secure localhost access:
   ```bash
   ssh -L 18789:localhost:18789 umbrel@your-umbrel-ip
   ```
2. Get your gateway token:
   - Right-click the OpenClaw app icon in Umbrel
   - Select "Show default credentials"
   - Copy the gateway token
3. Access the Control UI:
   ```
   http://localhost:18789/?token=YOUR_GATEWAY_TOKEN
   ```
4. Run the onboarding wizard to configure Telegram and AI models
5. Start chatting with your AI assistant in Telegram
6. Use voice messages and other interactive features

**Note:** SSH tunneling is required because OpenClaw's Control UI requires a secure context (HTTPS or localhost). The SSH tunnel makes it accessible as localhost on your machine.

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
