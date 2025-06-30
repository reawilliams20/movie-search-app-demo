# 🎬 Agentic Movie Search App Demo 

A simple React app that allows users to search for movies using the OMDb API and displays results with titles and posters. Created with GHCP Agent and tested with Playwright MCP.

## 🚀 Features

- 🔍 Search movies by title
- 🖼️ Display movie posters, titles, and release years
- ⚡ Built with React, TypeScript, and Vite
- 🎨 Responsive and clean UI

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

## 🛠️ Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/your-username/movie-search-app-demo.git
cd movie-search-app
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

### 4. **Enable GitHub Copilot Agent Mode**
- Open VS Code
- Go to Settings → Search `chat.agent.enabled` → Enable it
- Open Copilot Chat → Switch to **Agent Mode**

### 3. **Install Playwright MCP**
```bash
code --add-mcp '{"name":"playwright","command":"npx","args":["@playwright/mcp@latest"]}'
```
- Or manually add to `settings.json`:
```json
"mcp.servers": {
  "playwright": {
    "command": "npx",
    "args": ["@playwright/mcp@latest", "--browser", "msedge"]
  }
}
```
- Start the server via Command Palette: `MCP: List Servers` → Select `playwright`

### 4. **Build the Web App with Copilot**
Use **Copilot Ask** or **Edit Mode** to:
- Scaffold components
- Add a search bar
- Fetch movie data from OMDb API
- Display results

Example prompt:
> "Using the latest UI, Create a React component that fetches movies from OMDb API and displays them in a grid."
> "Update the web app so that it is responsive to browser screens"

### 5. **Generate Tests with Copilot + MCP**
Use **Copilot Agent Mode** to:
- Navigate to the app
- Type in the search bar
- Validate that results appear

Example prompt:
> "Generate a Playwright test that searches for 'Garfield' and verifies the movie appears."

Copilot will:
- Use MCP to open the browser
- Interact with the UI
- Generate a test like:
```ts
test('Search for Garfield', async ({ page }) => {
  await page.goto('http://localhost:5173');
  await page.getByPlaceholder('Search movies...').fill('Garfield');
  await page.keyboard.press('Enter');
  await expect(page.getByText('Garfield')).toBeVisible();
});
```

### 6. **Run and Validate the Test**
```bash
npx playwright test
```


