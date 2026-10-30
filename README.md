# Krishna Gupta — Personal Developer Portfolio

A responsive personal developer portfolio website developed across Lectures 9, 10, 13, 14, and 15, integrating modern web design, client-side interactivity, REST API connectivity, and LLM-powered chatbot capabilities.

## Live Demo & Repository
- **GitHub Repository**: [portfolio](https://github.com/krishnagupta/portfolio)
- **Deployment Platform**: Vercel

## Architecture & Features
1. **Semantic HTML5 & Responsive Design (Lecture 9)**:
   - Structured layout with Header, Main (`#about`, `#skills`, `#projects`), and Footer.
   - Clean CSS design with custom properties, blue/white/gold palette, and smooth link hover effects.
   - 100% compliant with W3C standards without inline styling.
2. **Interactive Dark Mode (Lecture 10)**:
   - Real-time theme toggle between light and dark mode with state-aware button text.
3. **Live Weather Checker (Lecture 14)**:
   - Dynamic real-time weather querying using OpenWeatherMap API with temperature, weather condition description, and humidity.
   - Comprehensive error handling for invalid cities (404), unauthorized keys (401), and rate limits (429).
4. **AI-Powered Portfolio Chatbot (Lecture 15)**:
   - Client-side conversational assistant powered by GroqCloud (`llama-3.1-8b-instant`).
   - Secure separation of API credentials via `config.js` and `.gitignore`.

## Project Structure
```
portfolio/
├── index.html        # Main HTML structure
├── style.css         # Core website styling and responsive layout
├── script.js         # Theme toggle and Weather API integration
├── chatbot.css       # Chatbot interface styling
├── chatbot.js        # Groq chat completion API handler
├── config.js         # API key and model configuration (git-ignored)
├── .gitignore        # Prevents committing API keys
├── page-audit.md     # Factual claim verification audit
└── README.md         # Project documentation
```

## Running Locally
Open `index.html` directly in Google Chrome or any modern browser:
```bash
start index.html
```
