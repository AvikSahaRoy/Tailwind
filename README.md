# Tailwind css

## Install Tailwind CSS with Vite

- Step 1 (Create Vite):
    ```
    npm create vite@latest my-project -- --template react
    ```
    ```
    cd my-project
    ```

- Step 2 (Install Tailwind CSS):
    ```
    npm install -D tailwindcss postcss autoprefixer
    ```
    ```
    npx tailwindcss init -p
    ```

- Step 3 (tailwind.config.js):
    ```
    /** @type {import('tailwindcss').Config} */
    export default {
    content: [
        "./index.html",
        "./src/**/*.{js,ts,jsx,tsx}",
    ],
    theme: {
        extend: {},
    },
    plugins: [],
    }
    ```

- Step 4 (./src/index.css):
    ```
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
    ```

- Step 5 (run project):
    ```
    npm run dev
    ```

## Start using Tailwind in your project
#### App.jsx
```
export default function App() {
  return (
    <h1 className="text-3xl font-bold underline">
      Hello world!
    </h1>
  )
}
```