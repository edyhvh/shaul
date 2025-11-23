# Shaul

A digital project to compile explanations and commentaries on the scriptures, inspired by the apostle Shaul (Paul).

## About the Project

Shaul is a digital platform that seeks to organize and share the understanding we receive from Elohim about the scriptures. The goal is to understand how the apostles thought about the scriptures, so that, if Elohim permits, we can make drash `דְּרַשׁ` in the same way they did, always keeping our eyes fixed on YESHUA HA'MASHIAJ.

## Main Objective

The objective of Shaul, the apostle, was to know and teach others who the Messiah is. This project seeks to follow that same purpose: to understand and share knowledge about the scriptures through the Ruaj, just as He who is the Word itself (Yeshua) did.

## Quick Start

### Requirements

- Node.js v22 or higher
- npm v10.9.2 or higher
- Git

### Clone the Repository

```bash
git clone <your-repository-url>
cd shaul
```

### Installation

Install the project dependencies:

```bash
npm install
```

### Local Development

Start the development server with hot-reload:

```bash
npm start
```

The site will be available at `http://localhost:8080`

### Build

Build the static site:

```bash
npm run build
```

The generated files will be in the `public/` directory.

### Deploy to Vercel

1. **Create a Vercel account** at [vercel.com](https://vercel.com) if you don't have one

2. **Install Vercel CLI** (optional, for command line deployment):
   ```bash
   npm i -g vercel
   ```

3. **Deploy via Vercel Dashboard**:
   - Go to [vercel.com/new](https://vercel.com/new)
   - Import your GitHub repository
   - Vercel will automatically detect the project settings
   - The build command is already configured: `npm run vercel-build`
   - The output directory is `public`
   - Click "Deploy"

4. **Deploy via CLI** (alternative):
   ```bash
   vercel
   ```
   Follow the prompts to link your project and deploy.

5. **Configure your domain** (optional):
   - In your Vercel project settings, go to "Domains"
   - Add your custom domain
   - Update the `baseUrl` in `quartz.config.ts` to match your domain

Your site will be live and automatically rebuild on every push to your main branch.

## Acknowledgments

Created with [Quartz v4.5.2](https://quartz.jzhao.xyz/) © 2025

- [Quartz Discord Community](https://discord.gg/cRFFHYye7t)
- [Quartz GitHub Repository](https://github.com/jackyzha0/quartz)

---

**SHALOM**
