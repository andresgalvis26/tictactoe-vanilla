# Tic Tac Toe - JavaScript Vanilla

Un juego clásico de Tres en Línea con tableros multigaga, modo contra IA, múltiples temas y estadísticas persistentes.

Desarrollado por **Andrés Galvis**.

## Características

### Juego
- **4 tamaños de tablero**: 3x3 (3 en línea), 4x4, 5x5 y 6x6 (4 en línea)
- **3 modos de juego**: 1 vs 1, vs IA (Fácil), vs IA (Difícil - Minimax)
- Generación dinámica de combinaciones ganadoras según el tamaño del tablero
- Resaltado de celdas ganadoras con animación
- Detección automática de fin de partida

### Visuales
- **4 temas intercambiables**: Default, Oscuro, Océano, Atardecer
- Animación de colocación de ficha (escala + rotación)
- Vista previa de la ficha al pasar el mouse (hover preview)
- Brillo dinámico en el tablero según el turno
- Confetti al ganar (60 piezas con colores aleatorios)
- Diseño glassmorphism con fondo gradiente
- Totalmente responsive

### Funcionalidades extra
- **Efectos de sonido** con Web Audio API (activar/desactivar)
- **Estadísticas persistentes** guardadas en localStorage
- **Historial de movimientos** con coordenadas por jugada
- Sistema de puntuación durante la sesión
- Footer con créditos del desarrollador
- Sin dependencias externas

## Cómo usar

### Servidor local
```bash
# Con Python
python -m http.server 8000

# Con Docker
docker build -t tictactoe .
docker run -d -p 8080:80 tictactoe
```

Luego visita `http://localhost:8000`.

### Descarga directa
1. Descarga `index.html` y `styles.css`
2. Abre `index.html` en tu navegador

## Controles

| Control | Descripción |
|---------|-------------|
| **Tema** | Cambia entre 4 estilos visuales |
| **Sonido** | Activa/desactiva efectos de sonido |
| **3x3 - 6x6** | Selecciona el tamaño del tablero |
| **1 vs 1 / vs IA** | Selecciona el modo de juego |
| **Nueva Partida** | Reinicia el tablero (mantiene puntuación) |

> Nota: El modo IA solo está disponible en tablero 3x3.

## Tecnologías

- **HTML5**: Estructura semántica
- **CSS3**: CSS Grid, Flexbox, variables CSS, animaciones keyframes, glassmorphism, responsive design
- **JavaScript ES6+**: Algoritmo Minimax, Web Audio API, localStorage, manipulación dinámica del DOM

## Estructura

```
tictactoe-vanilla/
├── index.html       # Juego completo (HTML + JS)
├── styles.css       # Estilos, temas y animaciones
├── Dockerfile       # Imagen Docker con Nginx Alpine
├── .dockerignore
├── README.md
└── public/
    ├── tictactoe.ico
    └── tictactoe.png
```

## Docker

```bash
docker build -t tictactoe .
docker run -d -p 8080:80 tictactoe
```

## Licencia

MIT
