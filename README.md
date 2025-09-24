# StoryFoundry

A multi-model storytelling studio with cinematic animations, collaborative AI writing tools, and a community library.

## Live Demo

Visit the live application at [masondaking.xyz](https://masondaking.xyz)

## Features

- **Multi-AI Support**: Generate content with OpenAI, Anthropic, Google Gemini, or DeepSeek
- **Cinematic Landing**: Immersive animations and gradient effects
- **Local Authentication**: Secure, browser-based user sessions
- **AI Writing Studio**: Advanced prompt controls with tone, genre, and POV settings
- **Smart Feedback**: Automated dialogue and structure analysis
- **Text-to-Speech**: ElevenLabs integration for narration generation
- **Community Library**: Share and discover stories with ratings and comments
- **Debug Console**: Real-time request monitoring and troubleshooting

## Quick Start

```bash
npm install
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) to view the application.

## Scripts

- `npm run dev` - Start development server
- `npm run build` - Create production build
- `npm run preview` - Preview production build locally

## API Configuration

StoryFoundry requires API keys for full functionality:

1. Navigate to `/studio` in the application
2. Select your preferred AI provider
3. Enter your API key (stored locally only)
4. Add ElevenLabs key for text-to-speech features

### Supported Providers

| Provider | Model | Endpoint |
|----------|-------|----------|
| OpenAI | gpt-4o-mini | `api.openai.com/v1/chat/completions` |
| Anthropic | claude-3-5-haiku-latest | `api.anthropic.com/v1/messages` |
| Google Gemini | gemini-1.5-flash | `generativelanguage.googleapis.com` |
| DeepSeek | deepseek-chat | `api.deepseek.com/chat/completions` |
| ElevenLabs | Various voices | `api.elevenlabs.io/v1/text-to-speech` |

## Project Structure

```
├── docs/                 # Documentation
├── public/              # Static assets
├── src/
│   ├── components/      # React components
│   │   ├── debug/       # Debug console
│   │   ├── library/     # Story library
│   │   ├── navigation/  # Navigation components
│   │   ├── tts/         # Text-to-speech
│   │   ├── ui/          # UI components
│   │   └── workspace/   # Writing studio
│   ├── context/         # React context providers
│   ├── hooks/           # Custom React hooks
│   ├── lib/             # Utility libraries
│   ├── pages/           # Main application pages
│   ├── styles/          # Styling files
│   └── utils/           # Helper functions
├── index.html
├── package.json
└── vite.config.ts
```

## Security & Privacy

- All API keys stored in browser localStorage only
- No server-side data transmission
- Local authentication with hashed credentials
- Client-side session management

## Development

Built with:
- **React** + **TypeScript**
- **Vite** for build tooling
- **Tailwind CSS** for styling
- **Local Storage** for data persistence

## Debug Features

Press `Alt + D` or use the debug button to access:
- Request/response logging
- Error tracking
- Payload inspection
- Console filtering

---

**Made by Reno and Mason*
