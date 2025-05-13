# React-TS

A minimalist boilerplate for quickly launching React projects with TypeScript and Vite.

## Features

- ⚡ Vite for lightning-fast development and optimized builds
- 🔧 TypeScript for type safety and improved developer experience
- ⚛️ React for building modern user interfaces
- 🚀 Netlify deployment ready
- 🌐 Environment variable configuration for multi-environment support
- 🧩 Includes base components and pages:
  - Home and About pages
  - Footer
  - Navbar with Home and About navigation buttons
  - Ready-to-use dark mode toggle
  - Other QoL features and fixes like scroll-to-top upon page change, and fix error upon refresh on Netlify
  - Website link: https://reacttsdev.netlify.app/

## Getting Started

### Prerequisites

- node.js
- npm
- git

### Setup Instructions

#### 1. Clone the repository

```bash
git clone git@github.com:kevinesg/react-TS.git your-project-name
cd your-project-name
```

#### 2. Install dependencies

Run the following command to sync up with the installed packages (don't forget to activate your virtual env first):

```bash
cd project-name
npm install
```

#### 3. Configure environment variables

Edit the values in `.env`. Add other values if needed.

#### 4. Connect to your GitHub repository

Create your new GitHub repo first.

Don't forget to change `your-username` and `your-project-name` below.

```bash
cd .. # assuming you're previously in project-name/
rm -rf .git
git init
git remote add origin git@github.com:your-username/your-project-name.git
git add .
git commit -m "initialized project from react-TS template"
git branch -M main
git push -u origin main
```

### Note on Deployment

Make sure to link your GitHub repository to a new Netlify setup. The user should handle this step. Set the build command to `npm run build` and the publish directory to `dist`.

## Development

Start the development server:

```bash
npm run dev
```

Build for production:

```bash
npm run build
```

Preview the production build:

```bash
npm run preview
```

## Deployment

This template is configured for easy deployment to Netlify. Connect your GitHub repository to Netlify and set the build command to `npm run build` and publish directory to `dist`.

## Project Structure

```
.
├── LICENSE
├── README.md
└── project-name
    ├── index.html
    ├── netlify.toml            # Avoid error on refresh
    ├── package-lock.json
    ├── package.json
    ├── public                  # Static assets
    ├── scripts
    │   └── generate-static.js  # Create robots.txt and _redirects
    ├── src
    │   ├── components/         # React components
    │   ├── pages/              # Page components
    │   ├── App.tsx             # Main application component
    │   ├── main.tsx            # Application entry point
    ├── tsconfig.app.json
    ├── tsconfig.json
    ├── tsconfig.node.json
    └── vite.config.ts
```
