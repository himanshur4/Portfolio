# 🚀 React + Vite Portfolio Template

A modern, responsive portfolio template built with React, Vite, and TailwindCSS to showcase your projects, skills, and experience.

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

- [Node.js](https://nodejs.org/) (v18 or higher)
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/) or [pnpm](https://pnpm.io/)
- [Git](https://git-scm.com/)

## 🛠️ Installation & Setup

### 1. Clone the repository

```bash
git clone https://github.com/salehkhatri/portfolio_template.git
cd portfolio_template
```

### 2. Install dependencies

Using npm:

```bash
npm install
```

Or, using yarn:

```bash
yarn
```

Or, using pnpm:

```bash
pnpm install
```

### 3. Start development server

```bash
npm run dev
```

This will start the development server at `http://localhost:5173` (or another port if 5173 is already in use).


## 🏗️ Building for Production

When you're ready to build your portfolio for production, run:

```bash
npm run build
```

This will generate optimized production files in the `dist` directory.

To preview the production build locally:

```bash
npm run preview
```

## 🚀 Deployment

### Netlify

1. Create a new site in Netlify
2. Connect to your GitHub repository
3. Set the build command to `npm run build`
4. Set the publish directory to `dist`

### Vercel

1. Install Vercel CLI (optional):

   ```bash
   npm install -g vercel
   ```

2. Deploy using Vercel CLI:

   ```bash
   vercel
   ```

   Or, simply connect your GitHub repository through the Vercel dashboard.

## 🔧 Customization

### Styling

This template uses TailwindCSS for styling. The theme is already customized with elegant typography and colors:

```javascript
import defaultTheme from "tailwindcss/defaultTheme.js";
/** @type {import('tailwindcss').Config} */
export default {
  content: ["./index.html", "./src/**/*.{js,ts,jsx,tsx}"],
  theme: {
    extend: {
      fontFamily: {
        // Clash Display for hero/headlines
        display: ["Clash Display", ...defaultTheme.fontFamily.sans],
        // Cabinet Grotesk for titles/subheadings
        title: ["Cabinet Grotesk", ...defaultTheme.fontFamily.sans],
        // General Sans for body text
        sans: ["General Sans", ...defaultTheme.fontFamily.sans],
      },
      colors: {
        primary: {
          // Rich black with slight warmth
          DEFAULT: "#111111",
          50: "#FAFAFA",
          100: "#F5F5F5",
          200: "#E5E5E5",
          300: "#D4D4D4",
          400: "#A3A3A3",
          500: "#737373",
          600: "#525252",
          700: "#404040",
          800: "#262626",
          900: "#171717",
        },
      },
      spacing: {
        18: "4.5rem",
        88: "22rem",
      },
      // Extended line heights for better typography
      lineHeight: {
        relaxed: "1.75",
        loose: "2",
      },
      // Custom letter spacing
      letterSpacing: {
        snug: "-0.015em",
        medium: "0.015em",
        wide: "0.025em",
      },
    },
  },
  plugins: [],
};
```

You can further customize this configuration to match your personal brand or preferences.

### Components

All components are located in the `src/components` directory. You can modify them to suit your needs or create new ones.

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- [React](https://reactjs.org/)
- [Vite](https://vitejs.dev/)
- [TailwindCSS](https://tailwindcss.com/)
- [React Icons](https://react-icons.github.io/react-icons/)

---

