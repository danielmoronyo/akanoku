# 🧩 Akanoku — El Sudoku d'Almudena

Juego de Sudoku en el navegador, con la ayuda de **Almudena**, una compañera que te guía y reacciona según cómo vayas. Sin instalación, sin backend: un único archivo HTML.

![Almudena](./images/almudena-character.png)

## ✨ Características

- **Tres tamaños de tablero**: Mini 4×4, Ràpid 6×6 y Clàssic 9×9.
- **Cinco niveles de dificultad**: Infantil (4×4), Fàcil, Mitjà, Difícil y Expert.
- **Tres vidas**: hasta 3 errades antes de fallar la partida.
- **Pistas**: 3 ayudas por partida que rellenan una casilla correcta.
- **Mode anotacions**: apunta candidatos en cada casilla sin comprometerte.
- **Desfer / Esborrar** para rectificar sobre la marcha.
- **Comprovar**: verifica el tablero al momento.
- **Cronòmetre** y contador de errores visibles en todo momento.
- **Multilingüe**: Valencià, Español, English, Français y Deutsch.
- **Totalmente offline**: no usa CDN, fuentes externas ni analytics. Funciona abriendo el archivo directamente.

## 🚀 Cómo jugar

La forma más fácil es abrirlo en el navegador:

1. Clona el repositorio y entra en la carpeta.
2. Abre `index.html` con doble clic.

Si prefieres un servidor local:

```bash
python3 -m http.server 8000
# y visita http://localhost:8000
```

## 🌐 Publicar en GitHub Pages

1. Ve a **Settings → Pages** en el repositorio.
2. En *Source* elige **Deploy from a branch**.
3. Selecciona la rama `main` y la carpeta `/ (root)`.
4. Guarda: en unos segundos tendrás la URL pública del juego.

## 📁 Estructura

```
akanoku/
├── index.html   # Juego completo (HTML + CSS + JS en un solo archivo)
├── images/      # Ilustraciones de Almudena (personaje, pensando, celebrando)
└── README.md
```

## 🛠️ Notas técnicas

- El proyecto es un único `index.html` autocontenido (bundle generado con Vite + React).
- Las rutas de las imágenes son **relativas** (`./images/...`) para que funcione tanto en la raíz de un dominio como en una subcarpeta (por ejemplo `usuario.github.io/akanoku`).
- No requiere build ni dependencias para jugar.

## 📄 Licencia

Código e ilustraciones propiedad de su autor. Añade aquí la licencia que prefieras (por ejemplo MIT) si quieres que otros puedan reutilizarlo.
