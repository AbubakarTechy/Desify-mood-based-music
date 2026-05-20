 # Desify - Mood-Based Music Recommendation

A modern web application that recommends music based on your current mood using React and Vite.

## Overview

Desify is an intelligent music recommendation system that analyzes your mood and suggests personalized music tracks to match your emotional state. Whether you're feeling happy, sad, energetic, or calm, Desify has the perfect playlist for you.

## Features

- **Mood Detection**: Advanced mood recognition system
- **Smart Recommendations**: AI-powered music suggestions
- **User-Friendly Interface**: Intuitive and responsive design
- **Real-time Updates**: Live playlist generation

## Tech Stack

- **Frontend**: React 18 + Vite
- **Styling**: Tailwind CSS
- **State Management**: Redux Toolkit
- **API Integration**: Spotify Web API
- **Deployment**: Vercel

## Installation

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn package manager

### Steps

1. Clone the repository
   ```bash
   git clone https://github.com/AbubakarTechy/Desify-mood-based-music.git
   cd Desify-mood-based-music
   ```

2. Install dependencies
   ```bash
   npm install
   ```

3. Create environment variables
   ```bash
   cp .env.example .env.local
   ```

4. Add your Spotify API credentials to `.env.local`

5. Start the development server
   ```bash
   npm run dev
   ```

6. Open [http://localhost:5173](http://localhost:5173) in your browser

## Usage

1. **Select Your Mood**: Choose from various mood options on the dashboard
2. **Get Recommendations**: Click the recommend button to generate a playlist
3. **Preview Tracks**: Listen to track previews directly in the app
4. **Save Favorites**: Add your favorite tracks to your personal collection
5. **Share Playlists**: Share your mood-based playlists with friends

## Project Structure

```
src/
├── components/      # React components
├── pages/          # Page components
├── store/          # Redux store configuration
├── services/       # API services
├── hooks/          # Custom React hooks
├── styles/         # Global styles
└── utils/          # Utility functions
```

## Configuration

### Environment Variables

```env
VITE_SPOTIFY_CLIENT_ID=your_spotify_client_id
VITE_SPOTIFY_CLIENT_SECRET=your_spotify_client_secret
VITE_REDIRECT_URI=http://localhost:5173/callback
VITE_API_BASE_URL=https://api.spotify.com/v1
```

## Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint
- `npm run test` - Run tests

## API Reference

### Mood Detection Endpoint
```
GET /api/moods
```

### Get Recommendations
```
POST /api/recommendations
Body: { mood: string, limit: number }
```

### User Preferences
```
GET /api/user/preferences
PUT /api/user/preferences
```

## Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Code of Conduct

Please note that this project is released with a [Contributor Code of Conduct](CODE_OF_CONDUCT.md). By participating in this project you agree to abide by its terms.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Spotify Web API for music data
- React and Vite communities for excellent tools
- All contributors who have helped with code and suggestions

## Support

For support, email support@desify.com or open an issue on GitHub.

## Roadmap

- [ ] Mobile app development
- [ ] Social features for sharing playlists
- [ ] Machine learning mood prediction
- [ ] Integration with other music platforms
- [ ] Offline mode support
- [ ] Dark mode theme

## Authors

- **Abubakar Rasheed** - Initial work - [AbubakarTechy](https://github.com/AbubakarTechy)

---

Made with ❤️ by the Desify Team
