# 🎬 Movie Search App

A simple React app that allows users to search for movies using the OMDb API and displays results with titles and posters.

## 🚀 Features

- 🔍 Search movies by title
- 🖼️ Display movie posters, titles, and release years
- ⚡ Built with React and Vite
- 🎨 Responsive and clean UI

## 🛠️ Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/your-username/movie-search-app-demo.git
cd movie-search-app-demo
```

### 2. Install dependencies

```bash
npm install
```

### 3. Run the development server

```bash
npm run dev
```

The app will be available at `http://localhost:5173`.

## 🔧 Configuration

This app uses the OMDb API. The demo key `apikey=demo` is used by default, but you can replace it with your own key:

1. Sign up at OMDb API  
2. Replace the API key in `App.jsx`:

```js
const response = await fetch(`https://www.omdbapi.com/?apikey=YOUR_API_KEY&s=${query}`);
```

## 🧪 Testing (Optional)

You can integrate Playwright for end-to-end testing. Here's a basic example:

```bash
npx playwright test
```

## 🤖 GitHub Copilot Demo

This project is ideal for demonstrating:
- Copilot Agent Mode for generating tests  
- Copilot Edit Mode for refactoring  
- Copilot Ask Mode for code explanations  
- Playwright MCP for browser automation

### 🛠️ Tools Required:
- VS Code (v1.99+)
- Node.js (v18+)
- GitHub Copilot (with Agent Mode enabled)
- Playwright MCP (npx @playwright/mcp@latest)
- React + Vite (for the web app)

## 📁 Project Structure

```
movie-search-app/
├── src/
│   ├── components/
│   │   ├── SearchBar.jsx
│   │   ├── MovieList.jsx
│   │   └── MovieCard.jsx
│   ├── App.jsx
│   ├── main.jsx
│   └── index.css
├── .gitignore
├── README.md
```

## 📄 License

This project is open-source and available under the MIT License.

