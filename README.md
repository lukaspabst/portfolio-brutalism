# LUKAS PABST — NEO BRUTALIST PORTFOLIO

A high-performance, neo-brutalist portfolio website built with **Astro**.
Features a custom heavy-contrast design system, theme switcher, and persistent preferences.

## ⚡ Tech Stack

- **Framework**: [Astro](https://astro.build)
- **Styling**: Vanilla CSS (Global Variables + Scoped)
- **Deployment**: Docker (Node Build -> Nginx Alpine)
- **State**: Vanilla JS (LocalStorage for Theme persistence)

## 🎨 Themes

Includes a custom **Theme Switcher** with 4 distinct aesthetics:
- **Cyber** (Default): Dark Mode, Neon Mint accents.
- **Neo**: Warm White, Bold Yellow.
- **Swiss**: Cool Grey, Klein Blue, Refined.
- **Voltage**: High Contrast Yellow/Magenta.

## 🚀 Development

```bash
# Install dependencies
npm install

# Start development server
npm run dev
```

## 🐳 Docker Production Build

The project includes a multi-stage `Dockerfile` (Node.js builder -> Nginx Alpine).

```bash
# Build image
docker build -t portfolio .

# Run container
docker run -p 80:80 portfolio
```

## 📁 Project Structure

```
src/
├── components/
│   └── neo/           # Neo-brutalist UI components (Card, Button, Switcher)
├── layouts/           # Global layout with Theme logic
├── pages/             # Route definitions
└── styles/
    └── global.css     # CSS Variables & Theme Definitions
```
