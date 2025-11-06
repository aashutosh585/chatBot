# 🤖 AI ChatBot - React + Vite

A modern AI-powered chatbot built with React and Vite, integrated with Google's Gemini AI API. Get instant intelligent responses to any question with a beautiful, responsive interface.

![ChatBot Demo](https://img.shields.io/badge/Status-Live-green) ![React](https://img.shields.io/badge/React-18+-blue) ![Vite](https://img.shields.io/badge/Vite-5+-yellow)

## ✨ Features

- 🧠 **AI-Powered** - Integrated with Google Gemini 2.0 Flash API
- 💬 **Conversational Interface** - Natural chat experience
- 🎨 **Modern UI/UX** - Beautiful gradient design with smooth animations
- 📱 **Responsive Design** - Works perfectly on all devices
- 🟣 **Floating Widget** - Non-intrusive corner chatbot
- 📝 **Text Formatting** - Supports markdown-like formatting (bold, bullets, lists)
- ⚡ **Fast Performance** - Built with Vite for lightning-fast development
- 🔒 **Secure** - Environment variables for API key protection

## 🚀 Quick Start


### Prerequisites
- Node.js 16+ 
- npm or yarn
- Google Gemini API Key

### 1. Clone the Repository
```bash
git clone <your-repo-url>
cd chatBot
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Environment Setup
Create a `.env` file in the root directory:
```env
VITE_GEMINI_API_KEY=your_gemini_api_key_here
```

**Get your API key from:** [Google AI Studio](https://makersuite.google.com/app/apikey)

### 4. Run Development Server
```bash
npm run dev
```
Open [http://localhost:5173](http://localhost:5173) in your browser.

## 🛠️ Build & Deploy

### Build for Production
```bash
npm run build
```
This creates an optimized build in the `dist/` folder.

### Deploy
Upload the `dist/` folder contents to any static hosting service:
- **Vercel**: `vercel --prod`
- **Netlify**: Drag & drop the `dist` folder
- **GitHub Pages**: Upload to gh-pages branch

## 📁 Project Structure

```
chatBot/
├── src/
│   ├── components/
│   │   ├── ChatMessage.jsx    # Message formatting component
│   │   ├── ChatForm.jsx       # Input form component
│   │   └── ChatbotIcon.jsx    # Bot icon component
│   ├── App.jsx                # Main application
│   ├── index.css              # Global styles
│   └── main.jsx               # App entry point
├── public/
├── .env                       # Environment variables
└── package.json
```

## ⚙️ Configuration

### Customizing the Bot
- **Welcome Message**: Edit the welcome text in `App.jsx`
- **Styling**: Modify colors and layout in `index.css`
- **AI Responses**: Adjust API parameters in the `generateBotResponse` function

### API Configuration
```javascript
// In App.jsx - generateBotResponse function
generationConfig: {
  temperature: 0.7,     // Creativity (0-1)
  topK: 40,            // Response variety
  topP: 0.95,          // Response precision
  maxOutputTokens: 1024 // Response length
}
```

## 🎯 Usage

1. **Click the purple chat button** in the bottom-right corner
2. **Type your question** in the input field
3. **Press Enter or click send** to get AI responses
4. **Close** by clicking the X or chat button again

## 🔧 Development

### Available Scripts
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

### Key Dependencies
- **React 18+** - UI framework
- **Vite** - Build tool and dev server
- **Axios** - HTTP client for API calls
- **Google Gemini API** - AI responses

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🐛 Troubleshooting

### Common Issues
- **API Key Error**: Make sure your `.env` file has the correct `VITE_GEMINI_API_KEY`
- **Build Fails**: Run `npm install` to ensure all dependencies are installed
- **Chatbot Not Responding**: Check browser console for API errors

### Support
If you encounter issues, please open an issue on GitHub with:
- Error message
- Browser and version
- Steps to reproduce

---

**Made with ❤️ using React + Vite + Gemini AI**
