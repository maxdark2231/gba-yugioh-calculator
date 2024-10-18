# Yu-Gi-Oh! Calculator for GBA / Calculadora de Yu-Gi-Oh! para GBA

Este proyecto es una calculadora de puntos de vida para Yu-Gi-Oh! desarrollada para la consola Game Boy Advance (GBA). Incluye varias funciones como sumar y restar puntos de vida, lanzar un dado, lanzar una moneda, y reiniciar los puntos de vida.

This project is a life point calculator for Yu-Gi-Oh! developed for the Game Boy Advance (GBA) console. It includes several functions like adding and subtracting life points, rolling a die, flipping a coin, and resetting life points.

---

## Funciones Principales / Main Features

- **Sumar y Restar puntos de vida / Add and Subtract Life Points**: Los jugadores pueden seleccionar la cantidad de puntos que desean sumar o restar y aplicarlos a su total de puntos de vida. / Players can select the amount of points they want to add or subtract and apply it to their life point total.
- **Lanzar dado / Roll a Die**: Al presionar el botón L, se lanzará un dado que muestra un número entre 1 y 6. / Press the L button to roll a die that shows a number between 1 and 6.
- **Lanzar moneda / Flip a Coin**: Al presionar el botón R, se lanza una moneda que mostrará "Heads" (cara) o "Tails" (cruz). / Press the R button to flip a coin that will show either "Heads" or "Tails."
- **Reiniciar puntos de vida / Reset Life Points**: Presiona **Start** para reiniciar los puntos de vida de ambos jugadores a 8000. / Press **Start** to reset the life points of both players to 8000.
- **Reiniciar todo / Reset Everything**: Presiona **Select** para reiniciar todo, incluyendo los puntos de vida, la selección de puntos, y los resultados del dado y la moneda. / Press **Select** to reset everything, including life points, point selection, and the die and coin results.

---

## Controles / Controls

- **D-Pad Izquierda/Derecha / Left/Right**: Navega entre las opciones de puntos de vida disponibles (50, 100, 1000, 2000). / Navigate between the available life point options (50, 100, 1000, 2000).
- **D-Pad Arriba/Abajo / Up/Down**: Selecciona entre el Jugador 1 y el Jugador 2. / Select between Player 1 and Player 2.
- **A**: Suma los puntos de vida seleccionados al jugador activo. / Adds the selected life points to the active player.
- **B**: Resta los puntos de vida seleccionados al jugador activo. / Subtracts the selected life points from the active player.
- **L**: Lanza un dado (mostrando un número entre 1 y 6). / Rolls a die (showing a number between 1 and 6).
- **R**: Lanza una moneda (mostrando "Heads" o "Tails"). / Flips a coin (showing "Heads" or "Tails").
- **Start**: Reinicia los puntos de vida de ambos jugadores a 8000. / Resets the life points of both players to 8000.
- **Select**: Reinicia toda la partida, restableciendo los puntos de vida, la selección de puntos, y borrando los resultados del dado y la moneda. / Resets everything, including life points, point selection, and clears the die and coin results.

---

## Cómo Funciona / How It Works

El programa usa la librería de GBA para generar un modo de texto simple en la pantalla. A través de las funciones del sistema, puedes interactuar con los puntos de vida de dos jugadores, lanzar un dado o una moneda, y reiniciar el juego cuando sea necesario.

The program uses the GBA library to generate a simple text mode on the screen. Through the system functions, you can interact with the life points of two players, roll a die or flip a coin, and reset the game when needed.

### Descripción de las funciones principales del código / Description of the Main Functions

1. **`initTextMode()`**: Inicializa el modo de texto en la consola GBA. / Initializes text mode on the GBA console.
2. **`printStaticScreen()`**: Muestra el título y las instrucciones en la pantalla al iniciar. / Displays the title and instructions on the screen at the start.
3. **`updateLifePoints()`**: Muestra los puntos de vida actuales de los jugadores en la pantalla. / Displays the current life points of the players on the screen.
4. **`showPoints()`**: Muestra las opciones de puntos de vida disponibles (50, 100, 1000, 2000) y resalta la opción seleccionada. / Displays the available life point options (50, 100, 1000, 2000) and highlights the selected option.
5. **`modifyLifePoints(int add)`**: Modifica los puntos de vida del jugador seleccionado, ya sea sumando o restando puntos, según el botón presionado (A o B). / Modifies the selected player's life points, either adding or subtracting points based on the button pressed (A or B).
6. **`rollDice()`**: Simula el lanzamiento de un dado y muestra el resultado en la pantalla (1-6). / Simulates rolling a die and displays the result on the screen (1-6).
7. **`flipCoin()`**: Simula el lanzamiento de una moneda y muestra el resultado en la pantalla (Heads o Tails). / Simulates flipping a coin and displays the result on the screen (Heads or Tails).
8. **`resetAll()`**: Reinicia los puntos de vida, limpia los resultados del dado y la moneda, y restablece la selección de puntos a la opción por defecto. / Resets the life points, clears the die and coin results, and resets the point selection to the default.

---

## Cómo Editar el Código / How to Edit the Code

El código es fácil de editar y modificar según tus necesidades. Aquí algunos puntos clave que puedes personalizar:  
The code is easy to edit and modify to suit your needs. Here are a few key areas you can customize:

1. **Modificar los puntos de vida iniciales / Modify the Initial Life Points**:
   - Los puntos de vida de ambos jugadores están inicializados en `8000`. Si deseas cambiar este valor por defecto, puedes editar las variables `player1LP` y `player2LP` en la función `resetAll()`. / The life points of both players are initialized to `8000`. If you want to change this default value, you can edit the variables `player1LP` and `player2LP` in the `resetAll()` function.

   ```c
   player1LP = 8000;  // Cambia este valor por otro si quieres un inicio diferente / Change this value to another if you want a different starting amount
   player2LP = 8000;
