# 🚀 AI-Powered Stock & Crypto Analyzer

A comprehensive, real-time financial analysis tool powered by Google's Gemini Flash 2.0 AI, featuring advanced technical indicators, news sentiment analysis, and interactive visualizations.

![Stock Analyzer](https://img.shields.io/badge/Version-2.0.0-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![AI Powered](https://img.shields.io/badge/AI-Gemini%20Flash%202.0-orange.svg)
![Status](https://img.shields.io/badge/Status-READY-brightgreen.svg)

## 🎉 **CLEAN, SIMPLIFIED, FULLY FUNCTIONAL**

### 🚀 **Quick Start**
**Simply open:** [`index.html`](index.html) - **Zero configuration required!**

**That's it!** No setup, no dependencies, no configuration needed. Just open and start analyzing stocks with AI.

## ✨ Features

### 🤖 AI-Powered Analysis
- **Gemini Flash 2.0 Integration**: Advanced AI analysis with multi-step reasoning
- **Multiple Analysis Types**: Quick analysis, detailed reports, price predictions, news correlation
- **Intelligent Prompting**: Context-aware prompts for accurate financial insights
- **Fallback System**: Mock analysis when API is unavailable

### 📊 Real-Time Data & Visualization
- **Live Stock/Crypto Data**: Real-time price feeds via Yahoo Finance API
- **Interactive Charts**: Chart.js powered visualizations with technical indicators
- **Technical Analysis**: SMA, RSI, MACD, Bollinger Bands, Stochastic Oscillator
- **Price Alerts**: Visual indicators for significant price movements

### 📰 News & Sentiment Analysis
- **News Integration**: Real-time financial news via NewsAPI
- **Sentiment Analysis**: AI-powered sentiment scoring of news articles
- **Correlation Analysis**: News sentiment vs. price movement correlation
- **Impact Assessment**: Quantified news impact on stock prices

### 🎯 Advanced Features
- **Watchlist Management**: Track multiple symbols with real-time updates
- **Export Capabilities**: PDF reports, JSON data, CSV exports
- **Auto-Refresh**: Configurable automatic data updates
- **Performance Monitoring**: Built-in performance tracking and optimization
- **Keyboard Shortcuts**: Full keyboard navigation support

### 🎨 User Experience
- **Dark/Light Themes**: Automatic theme switching with preference saving
- **Responsive Design**: Mobile-first design that works on all devices
- **Accessibility**: WCAG compliant with screen reader support
- **Progressive Enhancement**: Works without JavaScript (basic functionality)

## 🚀 Quick Start

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- Internet connection for real-time data
- Optional: Gemini API key for AI analysis
- Optional: NewsAPI key for real news data

### Installation

1. **Download or Clone**
   ```bash
   git clone https://github.com/yourusername/stock-crypto-analyzer.git
   cd stock-crypto-analyzer
   ```

2. **Open and Use**
   ```bash
   # Simply open the file in any modern browser
   open index.html
   # or double-click index.html
   ```

**That's it!** No server setup, no dependencies, no configuration needed.

### API Configuration (Optional)

- **Gemini API key is pre-configured** for immediate testing
- Get your own free Gemini API key from [Google AI Studio](https://makersuite.google.com/app/apikey)
- Enter your key in the API Configuration section for production use

### First Analysis

1. **Enter a Symbol**: Type a stock ticker (e.g., AAPL, TSLA) or crypto symbol (e.g., BTC-USD)
2. **Select Time Period**: Choose from 1 day to 2 years
3. **Choose Analysis Type**: Quick, Detailed, Prediction, or News Correlation
4. **Click Analyze**: Or press `Ctrl + Enter`

## 📁 Project Structure

```
stock-crypto-analyzer/
├── index.html              # 🚀 Main application (self-contained)
├── README.md              # 📖 Documentation
├── PROJECT-SUMMARY.md     # 📋 Project overview
└── SOLUTION.html          # 🔧 Problem resolution guide
```

**Clean and Simple:** Everything you need in just 4 files!

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl + Enter` | Run analysis |
| `Ctrl + R` | Refresh data |
| `Ctrl + E` | Export analysis |
| `Ctrl + W` | Add to watchlist |
| `Alt + 1-9` | Select watchlist item |
| `F1` | Show help |
| `Escape` | Close modals |

## 🔧 Configuration

### API Configuration
The application supports multiple API providers:

```javascript
// In js/config.js
const CONFIG = {
    YAHOO_FINANCE_API: 'https://query1.finance.yahoo.com/v8/finance/chart/',
    NEWS_API: 'https://newsapi.org/v2/everything',
    GEMINI_API: 'https://generativelanguage.googleapis.com/v1beta/models/gemini-2.0-flash-exp:generateContent',
    CACHE_DURATION: 5 * 60 * 1000, // 5 minutes
    UPDATE_INTERVAL: 5 * 60 * 1000  // 5 minutes
};
```

### Customization
- **Themes**: Modify CSS custom properties in `css/styles.css`
- **Chart Colors**: Update `CONFIG.CHART_COLORS` in `js/config.js`
- **Analysis Types**: Add new analysis types in `js/llm.js`
- **Technical Indicators**: Extend `analysis.js` with new indicators

## 🧪 Testing

### Quick Test
1. Open `index.html` in your browser
2. Enter a stock symbol (e.g., AAPL, TSLA, BTC-USD)
3. Click "Analyze" or press Ctrl+Enter
4. Verify AI analysis appears

### Manual Testing Checklist
- [ ] Symbol validation (valid/invalid inputs)
- [ ] AI analysis generation (with real API)
- [ ] Price data display (real-time updates)
- [ ] Theme switching (dark/light modes)
- [ ] Responsive design (mobile/tablet/desktop)
- [ ] Keyboard shortcuts (Ctrl+Enter, Ctrl+R)
- [ ] News sentiment analysis
- [ ] Error handling (invalid symbols)

### Browser Compatibility
- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+
- ⚠️ Internet Explorer (not supported)

## 🔧 Troubleshooting

### Common Issues

**No Analysis Appearing**
- **Check**: Internet connection for API calls
- **Solution**: App includes fallback mock data
- **Verify**: Gemini API key in settings

**Slow Performance**
- **Cause**: Network latency for API calls
- **Solution**: App includes smart caching
- **Note**: First load may be slower

**Mobile Display Issues**
- **Solution**: Refresh page, app is fully responsive
- **Note**: All features work on mobile devices

### Getting Help

1. **Check Browser Console**: Press F12 → Console tab for any errors
2. **Verify Internet**: Ensure connection for API calls
3. **Test Different Symbols**: Try AAPL, GOOGL, TSLA, BTC-USD
4. **Clear Cache**: Refresh with Ctrl+F5 if needed

## 🔒 Security & Privacy

### Data Handling
- **No Server Storage**: All data processed client-side
- **Local Storage Only**: Preferences saved locally
- **API Key Security**: Keys stored in browser local storage
- **HTTPS Recommended**: Use HTTPS for production deployment

### API Security
- **Rate Limiting**: Built-in request throttling
- **Error Handling**: Graceful degradation on API failures
- **Fallback Data**: Mock data when APIs unavailable
- **Input Validation**: All user inputs validated

## 🚀 Deployment

### Static Hosting
Deploy to any static hosting service:

```bash
# Netlify
netlify deploy --dir=. --prod

# Vercel
vercel --prod

# GitHub Pages
# Push to gh-pages branch

# AWS S3
aws s3 sync . s3://your-bucket-name --delete
```

### Environment Variables
For production deployment, consider using environment variables:

```javascript
// For build systems
const GEMINI_API_KEY = process.env.GEMINI_API_KEY;
const NEWS_API_KEY = process.env.NEWS_API_KEY;
```

## 🤝 Contributing

### Development Setup
1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Make changes and test thoroughly
4. Commit with descriptive messages
5. Push and create a pull request

### Code Style
- Use ES6+ JavaScript features
- Follow existing naming conventions
- Add JSDoc comments for functions
- Maintain responsive design principles
- Test on multiple browsers

### Adding Features
1. **New Analysis Types**: Add to `js/llm.js`
2. **Technical Indicators**: Extend `js/analysis.js`
3. **UI Components**: Add to `js/ui.js` and `css/components.css`
4. **API Integrations**: Extend `js/api.js`

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Google Gemini**: AI analysis capabilities
- **Yahoo Finance**: Real-time financial data
- **NewsAPI**: Financial news integration
- **Chart.js**: Interactive visualizations
- **Font Awesome**: Icon library

## 📞 Support

- **Issues**: [GitHub Issues](https://github.com/yourusername/stock-crypto-analyzer/issues)
- **Discussions**: [GitHub Discussions](https://github.com/yourusername/stock-crypto-analyzer/discussions)
- **Email**: support@yourproject.com

## 🔮 Roadmap

### Version 1.1
- [ ] Portfolio tracking
- [ ] Advanced charting (candlestick, volume)
- [ ] More technical indicators
- [ ] Social sentiment analysis

### Version 1.2
- [ ] Real-time alerts
- [ ] Mobile app (PWA)
- [ ] Multi-language support
- [ ] Advanced export options

### Version 2.0
- [ ] Machine learning predictions
- [ ] Options analysis
- [ ] Fundamental analysis
- [ ] Community features

---

**Made with ❤️ for the financial analysis community**
