# PowerStackHub

A powerful development stack built with Expo and React Native.

## 🚀 Features

- Cross-platform support (Web, iOS, Android)
- Built with Expo Router for navigation
- TypeScript support
- Automatic GitHub Pages deployment

## 📦 Installation

```bash
npm install
```

## 🛠️ Development

```bash
# Start development server
npm start

# Run on web
npm run web

# Run on iOS
npm run ios

# Run on Android
npm run android
```

## 🌐 Web Deployment

The app is automatically deployed to GitHub Pages when you push to the main branch.

### Manual Build

```bash
# Build for web
npm run build:web
```

The built files will be in the `dist` folder.

## 📁 Project Structure

```
PowerStackHub/
├── app/                 # App screens and navigation
│   ├── _layout.tsx     # Root layout
│   └── index.tsx       # Home screen
├── assets/             # Static assets
├── dist/               # Built web files (generated)
├── .github/workflows/  # GitHub Actions
└── package.json        # Dependencies and scripts
```

## 🚀 GitHub Pages Setup

1. Push this repository to GitHub
2. Go to repository Settings > Pages
3. Set Source to "GitHub Actions"
4. The app will be automatically deployed on every push to main

## 📱 Live Demo

Once deployed, your app will be available at:
`https://[your-username].github.io/PowerStackHub`

## 🔧 Technologies Used

- Expo
- React Native
- TypeScript
- Expo Router
- GitHub Actions
- GitHub Pages