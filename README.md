# Gemini Voice Assistance

A futuristic voice assistant web application powered by Google's Gemini AI, featuring real-time audio interaction and a JARVIS-inspired quantum terminal interface.

## Features

- **Real-time Voice Interaction**: Speak naturally and receive audio responses from Gemini AI
- **Advanced AI Model**: Uses Gemini 2.5 Flash with native audio preview capabilities
- **Futuristic UI**: Quantum terminal design with dynamic status indicators
- **Speech Recognition**: Automatic transcription of user input
- **Audio Synthesis**: High-quality voice output with customizable voice (Zephyr)
- **Responsive Design**: Works on desktop and mobile devices
- **No Backend Required**: Pure client-side implementation

## Prerequisites

- Google AI API key with access to Gemini Live API
- Modern web browser with microphone access
- HTTPS connection (required for microphone access)

## Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/rootrsk/gemini-voice-assistance.git
   cd gemini-voice-assistance
   ```

2. Open `index.html` in your browser, or serve it locally:
   ```bash
   python -m http.server 8000
   ```

3. The application will prompt for microphone permissions when you click "BEGIN"

## API Configuration

The application uses the Gemini Live API. Ensure your Google AI API key has the necessary permissions for:
- `ai.live.connect`
- Audio modalities
- Speech configuration

## Deployment

### Vercel (Recommended)

1. Push your code to GitHub
2. Connect your repository to Vercel
3. Deploy automatically - no build step required

The included `vercel.json` configures Vercel for static deployment.

### Other Platforms

Since this is a static HTML file, you can deploy to any static hosting service:
- GitHub Pages
- Netlify
- Firebase Hosting
- AWS S3 + CloudFront

## Usage

1. Open the application in a supported browser
2. Click the "BEGIN" button to initialize
3. Grant microphone permissions when prompted
4. Start speaking - the AI will respond with voice
5. Status indicators show current state:
   - Purple: Idle
   - Blue: Listening
   - Orange: Thinking
   - Pink: Speaking
   - Red: Error

## Browser Support

- Chrome 120+
- Firefox 120+
- Safari 17+
- Edge 120+

## Architecture

- **Frontend**: Pure HTML5, CSS3, and JavaScript
- **AI Integration**: Google Gemini Live API
- **Audio Processing**: Web Audio API
- **UI Framework**: Custom CSS with CSS Variables

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

MIT License - see LICENSE file for details

## Disclaimer

This application requires a valid Google AI API key and may incur usage costs. Ensure you understand Google's terms of service and pricing before deployment.