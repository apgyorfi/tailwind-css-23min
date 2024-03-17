# Learn TailwindCSS in 23 minutes
Videó: https://www.youtube.com/watch?v=W-LDhPyv478
Forrás repo: https://github.com/jamezmca/crystal-maths

## Projekt inicializálása
*A projektben Vanilla Framework lesz használva, de a Tailwind CSS keretrendszertől függetlenül használható!*

Projekt neve: `tailwind-css-23min`

> Docs: https://tailwindcss.com/docs/guides/vite
1. `npm create vite@latest tailwind-css-23min`
2. Select a framework: `Vanilla`
3. Select a variant: `JavaScript`
4. Belépés a projekt könyvtárba: `cd tailwind-css-23min` 
5. Felesleges fájl törlése: `counter.js`
6. `styles.css` és `index.html` kiürítése
7. `main.js` fájl törlése
8. Tailwind CSS telepítése: `npm install -D tailwindcss postcss autoprefixer`
9. Tailwind CSS inicializálása: `npx tailwindcss init -p`
10. Tailwind CSS konfigurálása, az alábbi kód hozzáadása a `tailwind.config.js` fájlhoz *(eredeti felülírása)*:
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
11. Tailwind direktívák hozzáadása a `styles.css` fájlhoz:
    ```
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
    ```
12. `npm run dev`
13. `index.html` fájl másolása a [forrás repo](https://github.com/jamezmca/crystal-maths/blob/main/index_blank.html)ból