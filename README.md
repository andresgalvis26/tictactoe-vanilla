# 🎮 Tic Tac Toe - JavaScript Vanilla

Un juego clásico de Tres en Línea (Tic Tac Toe) implementado con HTML, CSS y JavaScript vanilla. Diseño moderno con efectos visuales y sistema de puntuación.

## ✨ Características

- 🎯 **Juego completo**: Lógica de victoria, empate y alternancia de turnos
- 🏆 **Sistema de puntuación**: Contador de victorias para cada jugador y empates
- 🎨 **Diseño moderno**: Interfaz con efectos glassmorphism y animaciones suaves
- ⚡ **Cero dependencias**: Solo HTML, CSS y JavaScript vanilla
- 📱 **Responsive**: Se adapta a diferentes tamaños de pantalla
- 🌟 **Efectos visuales**: Animaciones de hover, victoria y transiciones

## 🚀 Cómo usar

### Opción 1: Descarga directa
1. Descarga el archivo `index.html`
2. Abre el archivo en tu navegador web
3. ¡Comienza a jugar!

### Opción 2: Clonar repositorio
```bash
git clone https://github.com/tu-usuario/tic-tac-toe-vanilla.git
cd tic-tac-toe-vanilla
```

Luego abre `index.html` en tu navegador.

### Opción 3: Servidor local
Si prefieres usar un servidor local:

```bash
# Con Python 3
python -m http.server 8000

# Con Node.js (si tienes http-server instalado)
npx http-server

# Con PHP
php -S localhost:8000
```

Luego visita `http://localhost:8000`

## 🎮 Cómo jugar

1. **Objetivo**: Ser el primero en conseguir tres símbolos iguales en línea (horizontal, vertical o diagonal)
2. **Turnos**: Los jugadores alternan entre X y O
3. **Victoria**: El juego detecta automáticamente al ganador y resalta las celdas ganadoras
4. **Puntuación**: Se mantiene el conteo de victorias durante la sesión
5. **Nueva partida**: Click en "🔄 Nueva Partida" para reiniciar

## 🛠️ Tecnologías utilizadas

- **HTML5**: Estructura semántica
- **CSS3**: Estilos modernos con:
  - CSS Grid para el tablero
  - Flexbox para el layout
  - Gradientes y efectos glassmorphism
  - Animaciones y transiciones
- **JavaScript ES6**: Lógica del juego con:
  - Event listeners
  - Manipulación del DOM
  - Arrays y funciones de alto nivel
  - Gestión de estado

## 📁 Estructura del proyecto

```
tic-tac-toe-vanilla/
│
├── index.html          # Archivo principal (HTML + CSS + JS)
├── README.md           # Este archivo
└── screenshot.png      # Captura de pantalla (opcional)
```

## 🔧 Funcionalidades técnicas

### Detección de victoria
El juego evalúa 8 combinaciones posibles:
- 3 filas horizontales
- 3 columnas verticales  
- 2 diagonales

### Gestión de estado
```javascript
let board = ['', '', '', '', '', '', '', '', ''];
let currentPlayer = 'X';
let gameOver = false;
let scores = { X: 0, O: 0, draw: 0 };
```

### Eventos principales
- `click` en celdas para realizar movimientos
- `click` en botón reset para nueva partida
- Validación de movimientos válidos

## 🎨 Personalización

### Cambiar colores
Modifica las variables CSS para personalizar la paleta:

```css
/* Jugador X */
.player-x { color: #e74c3c; }

/* Jugador O */  
.player-o { color: #3498db; }

/* Fondo principal */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

### Modificar tamaño del tablero
Ajusta las dimensiones en la clase `.board`:

```css
.board {
    grid-template-columns: repeat(3, 120px); /* Celdas más grandes */
    grid-template-rows: repeat(3, 120px);
}
```

## 🚀 Mejoras futuras

- [ ] Modo de juego contra IA
- [ ] Sonidos y efectos de audio
- [ ] Diferentes tamaños de tablero (4x4, 5x5)
- [ ] Modo multijugador online
- [ ] Temas de colores intercambiables
- [ ] Historial de partidas
- [ ] Animaciones más elaboradas

## 🤝 Contribuciones

¡Las contribuciones son bienvenidas! Si quieres mejorar el proyecto:

1. Fork el repositorio
2. Crea una rama para tu feature (`git checkout -b feature/nueva-caracteristica`)
3. Commit tus cambios (`git commit -am 'Añadir nueva característica'`)
4. Push a la rama (`git push origin feature/nueva-caracteristica`)
5. Abre un Pull Request

## 📝 Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo `LICENSE` para más detalles.

## 👨‍💻 Autor

Creado con ❤️ por [Tu Nombre]

---

## 📸 Capturas de pantalla

![Tic Tac Toe Screenshot](screenshot.png)

*Interfaz principal del juego mostrando el tablero y sistema de puntuación*

---

⭐ ¡Si te gusta este proyecto, dale una estrella en GitHub!