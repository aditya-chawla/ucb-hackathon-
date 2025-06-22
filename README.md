# almAid - AI-Powered Emotional Support Companion

![almAid Logo](https://img.shields.io/badge/almAid-AI%20Companion-blue?style=for-the-badge&logo=heart)

almAid is an AI-powered, audio-first virtual assistant designed to help users understand emotionally intense global crises while offering emotional grounding through personalized meditations and breathing exercises. It uses voice inputs to interpret emotions and delivers both responsible news summaries and customized calming activities.

## 🌟 Features

### 🧠 AI-Powered Emotional Support
- **Voice & Text Input**: Natural conversation through both voice and text
- **Emotional Analysis**: AI-powered emotional tone detection and response
- **Personalized Suggestions**: Tailored recommendations based on emotional state
- **24/7 Availability**: Round-the-clock emotional support

### 📰 Crisis Information Dashboard
- **Real-time News**: Latest updates on global crises and humanitarian issues
- **Responsible Reporting**: Curated news with emotional sensitivity
- **Category Filtering**: Filter news by conflict, climate, health, humanitarian
- **Search Functionality**: Find specific topics or regions

### 🧘‍♀️ Calm Space
- **Guided Meditations**: 5-15 minute sessions for different needs
- **Breathing Exercises**: Interactive 4-7-8, Box Breathing, and more
- **Calming Sounds**: Ocean waves, forest ambience, white noise
- **Moving Visuals**: Beautiful animated backgrounds for relaxation

### 🎤 Voice Assistant (VAPI Integration)
- **Natural Voice Interaction**: Hands-free emotional support
- **Speech Recognition**: Real-time voice-to-text conversion
- **Emotional Voice Analysis**: Tone detection for better support
- **Audio Responses**: Voice output for accessibility

## 🚀 Quick Start

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn
- Modern web browser with microphone access

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd almAid
   ```

2. **Install dependencies**
   ```bash
   npm run install-all
   ```

3. **Set up environment variables**
   ```bash
   cp env.example .env
   ```
   
   Edit `.env` and add your API keys:
   - Get a free News API key from [newsapi.org](https://newsapi.org/)
   - Get a VAPI key from [vapi.ai](https://vapi.ai/) (optional)
   - Get an OpenAI key from [platform.openai.com](https://platform.openai.com/) (optional)

4. **Start the application**
   ```bash
   npm run dev
   ```

5. **Open your browser**
   Navigate to `http://localhost:3000`

## 📱 Usage Guide

### Getting Started
1. **Home Page**: Overview of features and quick access to main functions
2. **Crisis Info**: Browse latest news with filtering and search
3. **Calm Space**: Access meditation, breathing exercises, and calming sounds
4. **Assistant**: Chat with AI for emotional support and information

### Voice Features
- Click the microphone button to start voice input
- Speak naturally about your concerns or questions
- The AI will analyze your emotional tone and respond appropriately
- Use voice commands for hands-free interaction

### Breathing Exercises
- Choose from different breathing patterns
- Follow the visual guide with expanding/contracting circle
- Complete the recommended number of cycles
- Stop anytime with the stop button

### News Dashboard
- Browse news tiles similar to Chrome's Android app
- Filter by category (conflict, climate, health, humanitarian)
- Search for specific topics
- Click "Read More" to view full articles

## 🛠️ Technology Stack

### Frontend
- **React 18**: Modern UI framework
- **Framer Motion**: Smooth animations and transitions
- **Lucide React**: Beautiful icons
- **Styled Components**: Component-based styling
- **Axios**: HTTP client for API calls

### Backend
- **Node.js**: Server runtime
- **Express.js**: Web framework
- **VAPI**: Voice AI integration
- **News API**: Real-time news data
- **Socket.io**: Real-time communication

### Features
- **Responsive Design**: Works on desktop, tablet, and mobile
- **Progressive Web App**: Installable and offline-capable
- **Accessibility**: Screen reader support and keyboard navigation
- **Performance**: Optimized loading and smooth animations

## 🔧 Configuration

### Environment Variables

| Variable | Description | Required | Default |
|----------|-------------|----------|---------|
| `PORT` | Server port | No | 5000 |
| `NEWS_API_KEY` | News API key | Yes | - |
| `VAPI_API_KEY` | VAPI key for voice AI | No | - |
| `OPENAI_API_KEY` | OpenAI key for AI responses | No | - |

### API Endpoints

- `GET /api/health` - Server health check
- `GET /api/news` - Get crisis news
- `GET /api/news/:category` - Get news by category
- `POST /api/assistant/chat` - AI assistant chat
- `GET /api/calm-activities` - Get meditation and breathing exercises

## 🎨 Customization

### Themes
The application uses CSS custom properties for easy theming. Modify the color variables in `client/src/index.css`:

```css
:root {
  --primary-gradient: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  --secondary-gradient: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
  --accent-color: #667eea;
}
```

### Adding New Activities
To add new meditation or breathing exercises, modify the `getDemoActivities()` function in the respective components or connect to your own API.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [News API](https://newsapi.org/) for providing news data
- [VAPI](https://vapi.ai/) for voice AI capabilities
- [Unsplash](https://unsplash.com/) for beautiful images
- [Framer Motion](https://www.framer.com/motion/) for animations
- [Lucide](https://lucide.dev/) for icons

## 📞 Support

If you need help or have questions:
- Open an issue on GitHub
- Check the documentation
- Join our community discussions

## 🔮 Roadmap

- [ ] Real-time voice synthesis for AI responses
- [ ] User accounts and progress tracking
- [ ] Community features and support groups
- [ ] Mobile app (React Native)
- [ ] Integration with wearable devices
- [ ] Advanced emotional analytics
- [ ] Multi-language support

---

**Made with ❤️ for emotional well-being during challenging times** 