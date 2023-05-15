Proyecto base(0)

Usar para comenzar todo proyecto como base.

Pasos realizados:

"Todos estos pasos deben realizar en la carpeta que se guardara el proyecto. Recuerda que en el paso uno se creara una carpeta nueva, puedes hacer todo esto desde el CMD"

1. Empezar proyecto "npm create vite@latest"

	1.1  vanilla
	1.2  JS

2. "npm instal @vitejs/plugin-react -E"

3. "npm install react react-dom -E"

4. Agregar documento "vite.config.js"

import { defineConfig } from "vite";
import React from '@vitejs/plugin-react';

export default defineConfig({
    plugins: [React()]
})

5. cambiar el index.js a index.jsx y hacer esto en el script de index.html

6. Crea una carpeta llamada "src" y crea el documento "App.jsx" en donde se manejara la web.

export function App() {

    return (
        <main>
            <h1>App principal</h1>
        </main>
    );
}

7. Agrega la libreria "createRoot" al index.jsx y crea un constante para conectar con el index.html usando

import { createRoot } from 'react-dom/client';
import { App } from './src/App.jsx';

const root = createRoot(document.getElementById('app'));
root.render(<App />);

8. Agrega el inter "npm install standar -D"; e ingresa el codigo en "package.json".

"eslintConfig": {
  "extends": "./node_modules/standard/eslintrc.json"
}

9. Ejecuta en la consola npm run dev


