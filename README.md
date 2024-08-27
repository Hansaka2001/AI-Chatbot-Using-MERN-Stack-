
# AI Chatbot Using MERN Stack

This repository contains an AI Chatbot application inspired by ChatGPT, built using the MERN stack and OpenAI's API. The chatbot is customized to store each user's message in a database, with features to retrieve and delete messages.

## Features

- **Custom Chatbot:** Each user message is stored in a database and can be retrieved or deleted.
- **Security:** The application is secured using JWT Tokens, HTTP-Only Cookies, Signed Cookies, Password Encryption, and Middleware Chains.
- **MERN Stack:** Built with MongoDB, Express.js, React, and Node.js for a robust full-stack development experience.

## Frontend Setup: React + TypeScript + Vite

This project uses React with TypeScript and is powered by Vite for fast development. It includes a minimal setup for React to work seamlessly with Vite and supports Hot Module Replacement (HMR).

### Available Plugins

- **[@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md):** Uses [Babel](https://babeljs.io/) for Fast Refresh.
- **[@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc):** Uses [SWC](https://swc.rs/) for Fast Refresh.

### ESLint Configuration

For production applications, we recommend expanding the ESLint configuration to enable type-aware lint rules:

1. Configure the top-level `parserOptions` property:

   ```js
   export default {
     // other rules...
     parserOptions: {
       ecmaVersion: 'latest',
       sourceType: 'module',
       project: ['./tsconfig.json', './tsconfig.node.json'],
       tsconfigRootDir: __dirname,
     },
   }
   ```

2. Replace `plugin:@typescript-eslint/recommended` with `plugin:@typescript-eslint/recommended-type-checked` or `plugin:@typescript-eslint/strict-type-checked`.
3. Optionally, add `plugin:@typescript-eslint/stylistic-type-checked`.
4. Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and add `plugin:react/recommended` & `plugin:react/jsx-runtime` to the `extends` list.

---
