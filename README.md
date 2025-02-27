# Tailwind CSS Setup with Vite (Manual Method)

This guide explains how to install and configure Tailwind CSS with Vite manually without using `npx` commands.

## 📌 Prerequisites

- Node.js and npm installed
- A basic Vite project setup

## 🚀 Step 1: Install Dependencies

Run the following command to install Tailwind CSS, PostCSS, and Autoprefixer:

```bash
npm install -D tailwindcss postcss autoprefixer vite
```

# 🔧 Step 2: Create Tailwind Config File Manually
### Create a file named `tailwind.config.js` in the root of your project and add the following:
  
  ```bash
    /** @type {import('tailwindcss').Config} */
    module.exports = {
        content: ["*"],
        theme: {
          extend: {},
        },
        plugins: [],
      };
      
  ```

# 🔧 Step 3: Create PostCSS Config File Manually
### Create a file named `package.json` in the root and add:
  ```bash
    {
  "scripts": {
    "start": "vite"
  },
  "devDependencies": {
    "autoprefixer": "^10.4.20",
    "postcss": "^8.5.3",
    "tailwindcss": "^4.0.9",
    "vite": "^6.2.0"
  }
}

  ```

# 🎨 Step 4: Add Tailwind Directives to Your CSS
### In your main CSS file `(src/index.css or styles.css)`, add the following:
  ```bash
      @tailwind base;
      @tailwind components;
      @tailwind utilities;

  ```

# 🚀 Step 5: Start the Vite Development Server
### Run the following command to start your project:
  ```bash
      npm run dev
  ```

Follow This Process Step By Step -> Then Your Tailwind have ready to use
