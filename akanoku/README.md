# 🧩 Akanoku — El Sudoku d'Almudena

Juego de Sudoku para el navegador con la ayuda de **Almudena**, una compañera que te guía, te anima y celebra la victoria contigo. Sin instalación, sin backend, sin conexión: **un único archivo HTML**.

![Almudena](./images/almudena-character.png)

## ✨ Características

**Tablero y dificultad**
- Tres tamaños: **Mini 4×4**, **Ràpid 6×6** y **Clàssic 9×9**.
- Cinco niveles: **Infantil (4×4)**, **Fàcil**, **Mitjà**, **Difícil** y **Expert**.

**Ayudas para no atascarse**
- **Pistes**: 3 ayudas por partida que rellenan una casilla correcta.
- **Anotacions** (llapis): apunta candidatos sin comprometerte.
- **Desfer** y **Esborrar** para rectificar sobre la marcha.
- **Comprovar**: verifica el tablero al instante.
- **Resoldre**: muestra la solución completa.
- **Tres vidas**: hasta 3 errades.

**Personalización**
- **Estil de fitxes**: números 1‑9, **emojis divertits** (🐱🐶🦊🐼🐸🦁🐨🦉🦄) o **formes de colors**.
- **Tres temas**: Clàssic fusta, Pastel suau i Nit fosca (mode fosc).
- **So** activable/desactivable.
- **Pausa** en cualquier momento.

**Seguimiento**
- Cronòmetre, puntuació i comptador d'errades.
- **Estadístiques**: partides jugades, guanyades, millor temps i ratxa actual.
- **Compartir resultat** al porta-retalls.

**Idiomes**
Valencià · Español · English · Français · Deutsch

## 🚀 Cómo jugar

La forma más fácil es abrirlo en el navegador:

1. Clona el repositorio y entra en la carpeta.
2. Abre `index.html` con doble clic.

Si prefieres servirlo:

```bash
python3 -m http.server 8000
# visita http://localhost:8000
```

## 🌐 Publicar en GitHub Pages

1. Entra en **Settings → Pages**.
2. En *Source* elige **Deploy from a branch**.
3. Rama `main` · carpeta `/ (root)` → **Save**.

En uno o dos minutos el juego estará disponible en
`https://TU-USUARIO.github.io/akanoku/`.

## 📁 Estructura

```
akanoku/
├── index.html                      # Juego completo (HTML + CSS + JS en un solo archivo, ~300 KB)
├── images/
│   ├── almudena-character.png      # Almudena (avatar y favicon)
│   ├── almudena-thinking.png       # Almudena pensando (durante la partida)
│   └── almudena-celebrate.png      # Almudena celebrando (al ganar)
├── .nojekyll                       # Evita que GitHub Pages procese el sitio con Jekyll
├── .gitignore
└── README.md
```

## 🛠️ Notas técnicas

- Un único `index.html` autocontenido (bundle de **Vite + React 19** con todo el CSS y el JS embebidos).
- **Cero dependencias externas**: no usa CDNs, fuentes remotas ni analítica. Funciona igual en `file://`, en GitHub Pages o en cualquier hosting.
- Las rutas de las imágenes son **relativas** (`./images/...`) para que funcione tanto en la raíz de un dominio como en una subcarpeta como `usuario.github.io/akanoku`.
- No requiere `npm install` ni build para jugar: basta con abrir el HTML.

## 📄 Licencia

Código e ilustraciones son propiedad de su autor. Si quieres permitir la reutilización,
añade un archivo `LICENSE` (por ejemplo, MIT).
