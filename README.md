# Pacman Game 👻

Un clon clásico del juego Pacman creado con Python Turtle, parte de la colección **Free Python Games**.

## 📋 Descripción

Este es un juego arcade clásico donde controlas a Pacman a través de un laberinto, comiendo puntos mientras evitas a los fantasmas. El objetivo es conseguir la mayor puntuación posible sin ser atrapado.

## 🎮 Cómo Jugar

1. **Usa las flechas del teclado** para mover a Pacman:
   - `←` Flecha Izquierda: Mover a la izquierda
   - `→` Flecha Derecha: Mover a la derecha
   - `↑` Flecha Arriba: Mover hacia arriba
   - `↓` Flecha Abajo: Mover hacia abajo

2. **Come todos los puntos blancos** para aumentar tu puntuación
3. **Evita a los fantasmas rojos** - si te tocan, ¡pierdes!
4. El juego termina cuando un fantasma te atrapa

## 🎯 Mecánicas del Juego

- **Pacman (amarillo)**: Controlado por el jugador, se mueve por el laberinto
- **Fantasmas (rojos)**: 4 fantasmas que se mueven automáticamente de forma aleatoria
- **Puntos blancos**: Cada punto vale 1 punto
- **Laberinto azul**: Paredes que delimitan el movimiento
- **Sistema de puntuación**: Se muestra en la esquina superior derecha

## Extra
- Los fantasmas son más inteligentes

## 🔧 Requisitos

```bash
pip install freegames
```

## 🚀 Ejecución

```bash
python pacman.py
```

O si tienes instalado `freegames`:

```bash
python -m freegames.pacman
```

## 📦 Dependencias

- **Python 3.x**
- **turtle** (incluido en Python estándar)
- **freegames**: Librería que proporciona utilidades como `vector` y `floor`

## 🎲 Características Técnicas

- Ventana de juego: 420x420 píxeles
- Tamaño de celda: 20x20 píxeles
- Grid del laberinto: 20x20 celdas
- Velocidad de movimiento: 5 unidades por movimiento
- Velocidad de actualización: 100ms por frame
- Número de fantasmas: 4 (con posiciones iniciales en las esquinas)
- Detección de colisión: Distancia menor a 20 unidades

## 🗺️ Estructura del Laberinto

El laberinto está definido por un array de 400 elementos (20x20):
- `0`: Pared (azul)
- `1`: Camino con punto (blanco)
- `2`: Camino ya recorrido (sin punto)

## 🤖 Comportamiento de los Fantasmas

Los fantasmas se mueven de forma semi-aleatoria:
- Intentan continuar en su dirección actual
- Si encuentran una pared, eligen aleatoriamente una nueva dirección válida
- Cada fantasma tiene su propia velocidad y dirección inicial

## 📝 Créditos

Este código pertenece a **Free Python Games**, una colección de juegos simples implementados en Python para fines educativos.

🔗 [Free Python Games - GitHub](https://github.com/grantjenks/free-python-games)

## 📄 Licencia

Este código es parte de Free Python Games. Consulta la licencia original del proyecto para más información.

---

**¡Diviértete jugando y trata de conseguir la mayor puntuación posible! 🏆**
